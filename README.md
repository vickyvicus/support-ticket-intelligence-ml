# Support Ticket Intelligence ML

An end-to-end machine learning project for analyzing customer support tickets.

## Problem Statement

Support teams receive many tickets every day. Manual prioritization can delay critical issues. This project uses machine learning to predict ticket priority, escalation risk, resolution time, and issue clusters.

## Module 1: Ticket Priority Classification

Goal: Predict support ticket priority using Decision Tree and Random Forest models.

## Tech Stack

- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Jupyter
- FastAPI later
- Docker later

## Project Status

- [ ] Dataset loaded
- [ ] EDA completed
- [ ] Decision Tree trained
- [ ] Random Forest trained
- [ ] Model evaluated
- [ ] Model saved

## Module 1: Ticket Priority Classification

### Goal
Predict support ticket priority using structured ticket information.

### Models Used
- Baseline Dummy Classifier
- Decision Tree Classifier
- Random Forest Classifier

### Features
- Ticket metadata
- Customer/ticket category fields
- Text-derived features such as text length, word count, and urgent keyword flag

### Evaluation
The models were evaluated using accuracy, macro F1-score, classification report, and confusion matrix.

### Key Learning
Random Forest generally performed better than a single Decision Tree because it combines multiple trees and reduces overfitting.


## Module 2: Escalation Risk Prediction

### Goal
Predict whether a support ticket is likely to be escalated.

### Model
Logistic Regression was used because escalation prediction is a binary classification problem.

### Target
The `is_escalated` label was synthetically generated using business-inspired rules based on customer tier, affected users, previous ticket count, urgent/error keywords, and ticket channel.

### Evaluation
The model was evaluated using precision, recall, F1-score, ROC-AUC, confusion matrix, and threshold tuning.

### Key Learning
For escalation prediction, recall is often more important than accuracy because missing a truly escalated ticket can delay urgent customer issues.


## Module 3: Resolution Time Prediction

### Goal
Predict the estimated time required to resolve a support ticket.

### Model
Linear Regression was used as the primary model to revise regression fundamentals. Ridge Regression and Random Forest Regressor were used for comparison.

### Target
The `resolution_time_hours` target was synthetically generated using business-inspired factors such as customer tier, affected users, previous ticket count, ticket channel, issue keywords, and escalation status.

### Evaluation
The model was evaluated using MAE, RMSE, R² score, actual vs predicted plot, and residual analysis.

### Key Learning
MAE is easier to explain to business users because it directly represents average prediction error in hours.