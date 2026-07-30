# Customer Churn Prediction System

## Project Overview
An end-to-end machine learning system that predicts which telecom customers 
are likely to churn (cancel their subscription), enabling proactive retention 
strategies. Built using the Telco Customer Churn dataset, covering data 
preprocessing, model training, experiment tracking, and deployment.

## Problem It Solves
Telecom companies lose significant revenue when customers churn without 
warning. Customer support and retention teams currently react only after 
a customer cancels, rather than intervening beforehand. This project 
identifies at-risk customers in advance using historical usage and account data.

## Target Users (Personas)
- **Retention Team Analyst** — needs a ranked list of at-risk customers to prioritize outreach.
- **Business/Product Manager** — needs churn trends and key churn drivers to inform pricing/product decisions.
- **Data Science Engineer** — needs a reproducible, trackable ML pipeline to iterate on models.

## Vision Statement
To give telecom businesses an accurate, explainable, and easily deployable 
tool that flags customers likely to churn, so retention teams can act before 
it's too late.

## Key Features / Goals
- Clean, leakage-free data preprocessing pipeline
- Handle class imbalance using SMOTE
- Compare multiple models (Logistic Regression, Random Forest, XGBoost)
- Track experiments and metrics using MLflow
- Serve predictions via a FastAPI backend
- Provide an interactive Streamlit dashboard for business users

## Success Metrics
- Model achieves recall ≥ 0.75 on churn class (minimizing missed at-risk customers)
- F1-score ≥ 0.65 on the churn class
- API response time < 500ms per prediction
- Dashboard usable by non-technical stakeholders without training

## Assumptions & Constraints
- Dataset is static (Kaggle Telco dataset), not live-streamed data
- Model retraining is manual, not automated (out of scope for this phase)
- Deployment is local/containerized, not on cloud infrastructure (yet)
- English-language, single-market (US telecom) data only