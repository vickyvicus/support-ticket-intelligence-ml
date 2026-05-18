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