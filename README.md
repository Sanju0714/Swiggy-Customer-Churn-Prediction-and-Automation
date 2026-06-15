# Swiggy Customer Churn Prediction & Campaign Automation

## Overview

This project predicts customer churn using Machine Learning and automates customer engagement campaigns using n8n. Customers likely to churn are identified and targeted with retention offers, while loyal customers receive appreciation messages.

## Problem Statement

Customer retention is a major challenge for food delivery platforms. Swiggy needs a system to identify customers at risk of churning and automatically engage them with personalized campaigns.

## Solution

Built an end-to-end pipeline that:

* Performs data validation and quality checks
* Generates automated profiling reports using YData Profiling
* Predicts customer churn using Random Forest Classifier
* Segments customers into High Risk and Low Risk categories
* Generates personalized campaign messages
* Automates email notifications using n8n

## Tech Stack

* Python
* Pandas
* Scikit-learn
* YData Profiling
* n8n
* Gmail Integration

## Workflow

Dataset → Data Validation → YData Profiling → Churn Prediction → Customer Segmentation → Campaign Generation → n8n Automation → Email Notification

## Business Logic

### High Risk Customers

* Churn = 1
* Action: 20% Discount Coupon

### Low Risk Customers

* Churn = 0
* Action: Customer Appreciation Message

## Model Performance

* Algorithm: Random Forest Classifier
* Accuracy: 98%
* Precision: 100%
* Recall: 86%
* F1 Score: 92%

## Project Structure

```text
Swiggy-Customer-Churn-Prediction-and-Automation/
│
├── data/
├── notebooks/
├── reports/
├── outputs/
├── n8n/
├── screenshots/
├── requirements.txt
└── README.md
```

## Screenshots

### n8n Workflow
<img width="2460" height="1042" alt="Screenshot 2026-06-15 201835" src="https://github.com/user-attachments/assets/9a2dc9aa-475a-4c08-abda-e4c4091dbbd4" />

### Email Automation
<img width="1874" height="936" alt="image" src="https://github.com/user-attachments/assets/91948b51-2e31-475f-b50d-fd645087d1fd" />

## How to Run

```bash
git clone <repository_url>
cd Swiggy-Customer-Churn-Prediction-and-Automation

pip install -r requirements.txt

jupyter notebook
```

Run notebooks in the following order:

1. 01_data_audit.ipynb
2. 02_ydata_profiling.ipynb
3. 03_data_validation.ipynb
4. 04_churn_prediction_model.ipynb

## Outputs

* Customer churn prediction model
* High Risk and Low Risk customer segmentation
* Automated campaign generation
* n8n email notification workflow

## Business Impact

* Identifies customers likely to churn
* Improves customer retention through targeted campaigns
* Automates customer engagement workflows
* Reduces manual effort through workflow automation

## Author

**Sanjana**
