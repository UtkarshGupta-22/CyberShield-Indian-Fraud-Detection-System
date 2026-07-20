<div align="center">

# CyberShield: Indian Fraud Detection System

### AI-Powered Fraud Detection Platform for India's Digital Banking Ecosystem

An intelligent fraud detection platform designed to identify suspicious financial transactions across **UPI**, **credit cards**, and **banking systems** using **Machine Learning**, **Ensemble Models**, and **Indian-specific behavioral intelligence**.

Built with **Python**, **Flask**, **Streamlit**, **Scikit-learn**, and **XGBoost**, CyberShield delivers real-time fraud risk assessment through an interactive dashboard and RESTful API.

---

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)

[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org)

[![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-EC6C00?style=for-the-badge)](https://xgboost.ai)

[![Flask](https://img.shields.io/badge/Flask-Backend-000000?style=for-the-badge&logo=flask)](https://flask.palletsprojects.com)

[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=for-the-badge&logo=streamlit)](https://streamlit.io)

[![Docker](https://img.shields.io/badge/Docker-Deployment-2496ED?style=for-the-badge&logo=docker)](https://docker.com)

[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

</div>

---

# Table of Contents

- About the Project
- Problem Statement
- Objectives
- Key Features
- System Architecture
- AI Pipeline
- Technology Stack
- Repository Structure
- Installation
- Running the Project
- REST API
- Machine Learning Models
- Datasets
- Dashboard
- Results
- Challenges
- Future Roadmap
- Skills Demonstrated
- Contributors
- License

---

# About the Project

CyberShield is an AI-powered fraud detection platform developed to address the rapidly evolving landscape of digital financial fraud in India.

Unlike traditional fraud detection systems that primarily focus on generic transaction behavior, CyberShield incorporates **Indian banking characteristics**, **UPI payment ecosystems**, **regional transaction patterns**, and **behavioral analytics** to improve fraud detection accuracy.

The system analyzes financial transactions in real time and estimates fraud probability using multiple machine learning models, enabling faster and more informed decision-making for banking institutions and digital payment platforms.

---

# Why CyberShield?

India has become one of the world's largest digital payment ecosystems with billions of transactions processed every month through:

- UPI
- Credit Cards
- Debit Cards
- Internet Banking
- Mobile Wallets

As digital transactions continue to grow, fraud techniques have become increasingly sophisticated. Traditional rule-based fraud detection systems often struggle to identify emerging attack patterns without generating excessive false positives.

CyberShield addresses this challenge by combining machine learning with domain-specific knowledge of India's financial ecosystem to provide intelligent, real-time fraud analysis.

---

# Problem Statement

Financial institutions face several challenges when detecting fraudulent transactions:

- Increasing transaction volume
- Rapidly evolving fraud techniques
- High false-positive rates
- Delayed fraud detection
- Lack of behavioral analysis
- Limited adaptation to regional payment patterns

These challenges become even more significant in India's fast-growing UPI ecosystem, where real-time transaction processing is essential.

CyberShield aims to overcome these limitations through an AI-driven, scalable fraud detection framework.

---

# Project Objectives

The primary objectives of CyberShield are to:

- Detect fraudulent financial transactions in real time.
- Support fraud analysis across multiple payment channels.
- Improve fraud detection accuracy using ensemble machine learning models.
- Reduce false positives while maintaining high fraud recall.
- Provide interactive dashboards for fraud analysts.
- Enable seamless integration through REST APIs.
- Support future expansion with additional financial datasets and models.

---

# Key Features

| Feature | Description |
|----------|-------------|
| Credit Card Fraud Detection | AI-based transaction risk analysis |
| UPI Fraud Detection | Detect suspicious UPI payment behavior |
| Bank Transaction Analysis | Risk estimation for banking transactions |
| Ensemble Machine Learning | Multiple models combined for improved performance |
| Interactive Dashboard | Streamlit-powered visualization |
| REST API | Flask backend for prediction services |
| Batch Prediction | CSV transaction analysis |
| Docker Support | Easy deployment across environments |
| Risk Scoring | Fraud probability estimation |
| Explainable Outputs | Risk levels with confidence scores |

---

# Project Highlights

- Real-time fraud detection
- Machine Learning ensemble models
- Credit card transaction analysis
- UPI transaction intelligence
- Banking transaction monitoring
- REST API integration
- Interactive Streamlit dashboard
- Docker deployment
- Batch transaction processing
- Modular project architecture
- Scalable design
- Production-ready deployment structure

---

# Use Cases

CyberShield can be adapted for multiple financial applications.

### Banking Institutions

- Transaction monitoring
- Suspicious activity detection
- Fraud prevention

### Digital Payment Platforms

- UPI payment validation
- Wallet transaction monitoring
- Payment risk assessment

### Financial Analysts

- Fraud investigation
- Transaction analytics
- Risk visualization

### Research & Education

- Machine learning experimentation
- Fraud analytics research
- Financial AI projects

---

# Repository Snapshot

| Category | Details |
|----------|---------|
| Domain | Financial Technology (FinTech) |
| Project Type | Machine Learning + Web Application |
| Backend | Flask |
| Frontend | Streamlit |
| Machine Learning | Scikit-learn, XGBoost |
| Deployment | Docker |
| Language | Python |

# System Architecture

CyberShield follows a modular architecture where every component is responsible for a specific stage of the fraud detection pipeline. The modular design allows individual models, APIs, and dashboards to be updated independently while maintaining a scalable and production-ready workflow.

```text
                           ┌──────────────────────────────┐
                           │     Client Application       │
                           │ Web / Dashboard / API Client │
                           └──────────────┬───────────────┘
                                          │
                                          ▼
                              Transaction Request
                                          │
                                          ▼
                          ┌─────────────────────────┐
                          │      Flask REST API      │
                          └────────────┬────────────┘
                                       │
                                       ▼
                        ┌────────────────────────────┐
                        │ Transaction Preprocessing  │
                        └────────────┬───────────────┘
                                     │
             ┌───────────────────────┼────────────────────────┐
             │                       │                        │
             ▼                       ▼                        ▼
    Credit Card Model        UPI Fraud Model       Bank Account Model
             │                       │                        │
             └──────────────┬────────┴──────────────┬─────────┘
                            ▼
                  Ensemble Decision Engine
                            │
                            ▼
                  Fraud Risk Probability
                            │
                            ▼
                 Risk Classification Engine
                            │
                            ▼
            Dashboard • API Response • Reports
```

---

# Fraud Detection Pipeline

Each incoming transaction passes through multiple processing stages before a final fraud probability is generated.

```text
Incoming Transaction

        │

        ▼

Data Validation

        │

        ▼

Feature Engineering

        │

        ▼

Data Normalization

        │

        ▼

Model Selection

        │

        ▼

Machine Learning Prediction

        │

        ▼

Fraud Probability Calculation

        │

        ▼

Risk Classification

        │

        ▼

Dashboard Visualization

        │

        ▼

Prediction API Response
```

---

# Overall Workflow

```text
Transaction

↓

Receive Request

↓

Validate Input

↓

Extract Features

↓

Select Appropriate Model

↓

Generate Fraud Probability

↓

Assign Risk Level

↓

Display Dashboard

↓

Store Prediction

↓

Generate Report
```

---

# Technology Stack

## Programming Language

- Python

---

## Machine Learning

- Scikit-learn
- XGBoost
- Random Forest
- Logistic Regression

---

## Backend

- Flask REST API

---

## Frontend

- Streamlit

---

## Data Processing

- Pandas
- NumPy

---

## Data Visualization

- Matplotlib

---

## Deployment

- Docker
- Docker Compose

---

## Development

- Jupyter Notebook
- Git
- GitHub

---

# Technology Summary

| Layer | Technologies |
|---------|-------------|
| Programming | Python |
| Machine Learning | Scikit-learn |
| Ensemble Learning | XGBoost, Random Forest, Logistic Regression |
| Backend | Flask |
| Frontend | Streamlit |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| Deployment | Docker |
| Version Control | Git, GitHub |

---

# Repository Structure

```text
CyberShield-Indian-Fraud-Detection-System/
│
├── data/
│   ├── datasets/
│   ├── processed_data/
│   └── sample_transactions/
│
├── models/
│   ├── trained_models/
│   ├── scalers/
│   └── encoders/
│
├── collab notebook/
│   ├── model_training.ipynb
│   └── experimentation.ipynb
│
├── app.py
├── dashboard.py
├── train.py
├── train_models.py
├── train_model.py
├── evaluate.py
├── simulate_flags.py
├── requirements.txt
├── docker-compose.yml
├── Dockerfile
└── README.md
```

---

# Core Modules

## 1. Fraud Detection Engine

The central prediction engine evaluates incoming financial transactions and estimates the probability of fraudulent behavior using trained machine learning models.

### Responsibilities

- Transaction Analysis
- Feature Processing
- Fraud Prediction
- Risk Scoring

---

## 2. Credit Card Fraud Module

Designed to identify suspicious credit card transactions by learning historical fraud patterns and transaction anomalies.

### Key Features

- Transaction amount analysis
- Merchant behavior analysis
- Temporal feature analysis
- Fraud probability estimation

---

## 3. UPI Fraud Detection Module

This module focuses on India's Unified Payments Interface (UPI), incorporating payment-specific features to identify potentially fraudulent digital transactions.

### Supported Scenarios

- Peer-to-peer payments
- Merchant payments
- New beneficiary transfers
- Device changes
- High-value UPI transactions

---

## 4. Banking Fraud Analysis Module

Analyzes banking transactions by considering customer behavior, transaction history, and account-related attributes to identify suspicious activity.

### Applications

- Internet Banking
- Mobile Banking
- Fund Transfers
- Account Monitoring

---

## 5. Machine Learning Ensemble

Instead of relying on a single model, CyberShield supports multiple algorithms that can be evaluated and combined for improved fraud detection performance.

Potential models include:

- Random Forest
- Logistic Regression
- XGBoost
- Gradient Boosting

The ensemble approach improves robustness and helps balance fraud detection performance with reduced false positives.

---

## 6. REST API

The Flask backend exposes prediction endpoints that allow external applications to integrate CyberShield into their workflows.

Typical API capabilities include:

- Single transaction prediction
- Batch transaction analysis
- Fraud probability estimation
- Risk classification
- Model information

---

## 7. Streamlit Dashboard

The interactive dashboard enables users to visualize fraud predictions and analyze transaction behavior in real time.

Dashboard capabilities include:

- Live prediction interface
- Fraud probability visualization
- Batch CSV upload
- Performance statistics
- Model insights
- Interactive charts

---

# Data Flow

```text
Transaction

↓

Feature Engineering

↓

Data Cleaning

↓

Scaling & Encoding

↓

Machine Learning Model

↓

Fraud Probability

↓

Risk Classification

↓

Dashboard / REST API

↓

Report Generation
```

---

# Design Principles

CyberShield was developed with the following software engineering principles in mind:

- Modular Architecture
- Scalability
- Maintainability
- Separation of Concerns
- API-First Design
- Reusable Machine Learning Pipeline
- Production-Oriented Deployment
- Extensible Model Architecture

---

# Getting Started

Follow the instructions below to set up CyberShield on your local machine.

---

# System Requirements

| Requirement | Recommended |
|-------------|-------------|
| Operating System | Windows / Linux / macOS |
| Python | 3.10+ |
| RAM | 8 GB Minimum (16 GB Recommended) |
| Storage | 2 GB Free Space |
| Docker | Optional |

---

# Installation

## 1. Clone the Repository

```bash
git clone https://github.com/UtkarshGupta-22/CyberShield-Indian-Fraud-Detection-System.git

cd CyberShield-Indian-Fraud-Detection-System
```

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Verify Installation

Check the installed packages.

```bash
pip list
```

You should have packages such as:

- Flask
- Streamlit
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib

---

# Running the Project

CyberShield consists of two primary components:

- Flask Backend API
- Streamlit Dashboard

---

## Start the Backend API

```bash
python app.py
```

The API will start locally.

Example:

```text
http://localhost:5000
```

---

## Launch the Dashboard

Open another terminal.

```bash
streamlit run dashboard.py
```

The dashboard is available at

```text
http://localhost:8501
```

---

# Dashboard Overview

The Streamlit dashboard provides an intuitive interface for interacting with the fraud detection models.

## Features

- Single Transaction Prediction
- Batch CSV Prediction
- Fraud Probability Visualization
- Risk Classification
- Model Performance Statistics
- Interactive Charts
- Prediction History
- Transaction Analysis

---

# Prediction Workflow

```text
Enter Transaction

↓

Validate Inputs

↓

Generate Features

↓

Load ML Model

↓

Fraud Prediction

↓

Risk Probability

↓

Dashboard Visualization

↓

Export Results
```

---

# Machine Learning Model Training

The repository includes training scripts for developing and evaluating fraud detection models.

## Train a Model

```bash
python train.py
```

or

```bash
python train_models.py
```

---

## Evaluate Model Performance

```bash
python evaluate.py
```

Typical evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

---

## Simulate Fraud Scenarios

Generate synthetic fraud alerts for testing.

```bash
python simulate_flags.py
```

This helps validate the prediction pipeline under different fraud scenarios.

---

# REST API

CyberShield exposes RESTful APIs that allow external systems to integrate fraud detection capabilities.

---

## Health Check

```http
GET /
```

Returns API status.

---

## Fraud Prediction

```http
POST /predict
```

Example Request

```json
{
  "amount": 15000,
  "transaction_type": "UPI",
  "merchant": "Electronics",
  "location": "Delhi"
}
```

Example Response

```json
{
  "fraud_probability": 0.92,
  "risk_level": "HIGH",
  "prediction": "Fraudulent"
}
```

---

## Batch Prediction

Upload a CSV containing multiple transactions.

The API returns predictions for every transaction along with fraud probability and assigned risk level.

---

# Project Configuration

Important project files

```text
app.py

dashboard.py

train.py

evaluate.py

simulate_flags.py

requirements.txt

docker-compose.yml
```

Machine learning models should be stored in

```text
models/
```

Training datasets should be placed inside

```text
data/
```

---

# Docker Deployment

CyberShield supports containerized deployment using Docker.

## Build Docker Image

```bash
docker build -t cybershield .
```

---

## Run Docker Container

```bash
docker run -p 5000:5000 -p 8501:8501 cybershield
```

---

## Docker Compose

```bash
docker-compose up --build
```

This starts both the backend API and the Streamlit dashboard simultaneously.

---

# Sample Project Workflow

```text
Prepare Dataset

↓

Feature Engineering

↓

Train ML Models

↓

Evaluate Performance

↓

Save Best Model

↓

Start Flask API

↓

Launch Streamlit Dashboard

↓

Predict Fraud

↓

Generate Reports
```

---

# Example Transaction

| Feature | Value |
|----------|-------|
| Amount | ₹25,000 |
| Payment Method | UPI |
| Bank | HDFC Bank |
| Merchant Category | Online Shopping |
| City | Bengaluru |
| Time | 10:30 PM |

Prediction

```text
Fraud Probability : 91.8%

Risk Level : HIGH

Prediction : Fraudulent
```

---

# Output Reports

CyberShield generates multiple outputs.

| Output | Description |
|----------|-------------|
| Prediction Report | Transaction-wise fraud prediction |
| Risk Summary | Fraud distribution |
| Charts | Interactive visualizations |
| CSV Export | Batch prediction results |
| Evaluation Metrics | Model performance |

---

# Screenshots

Create an `assets/` folder and place screenshots inside it.

```text
assets/

├── dashboard.png

├── prediction.png

├── analytics.png

├── batch_prediction.png

└── api_demo.png
```

Then reference them as follows.

```markdown
## Dashboard

![Dashboard](assets/dashboard.png)

---

## Prediction Interface

![Prediction](assets/prediction.png)

---

## Analytics

![Analytics](assets/analytics.png)

---

## Batch Prediction

![Batch Prediction](assets/batch_prediction.png)

---

## API Demonstration

![API](assets/api_demo.png)
```

---

# Deployment Options

CyberShield can be deployed in multiple environments.

- Local Development
- Docker
- AWS
- Azure
- Google Cloud Platform
- Railway
- Render
- DigitalOcean
- On-premise Servers

The modular architecture allows the backend and frontend to be deployed independently, making it suitable for both development and production environments.

---

# Machine Learning Pipeline

CyberShield leverages supervised machine learning techniques to classify financial transactions as **legitimate** or **fraudulent**. Instead of relying on fixed rules, the system learns transaction behavior from historical datasets and predicts the likelihood of fraud for unseen transactions.

The workflow is designed to be modular, enabling different fraud detection models to be trained, evaluated, and deployed independently.

---

# Model Development Workflow

```text
Raw Transaction Data
          │
          ▼
Data Cleaning
          │
          ▼
Feature Engineering
          │
          ▼
Encoding & Scaling
          │
          ▼
Train / Validation Split
          │
          ▼
Model Training
          │
          ▼
Performance Evaluation
          │
          ▼
Model Selection
          │
          ▼
Model Serialization
          │
          ▼
Flask API
          │
          ▼
Real-Time Predictions
```

---

# Machine Learning Models

CyberShield supports multiple supervised learning algorithms for fraud detection.

| Model | Purpose |
|---------|----------|
| Logistic Regression | Baseline classifier |
| Random Forest | Ensemble classification |
| XGBoost | Gradient boosting for complex fraud patterns |
| Voting / Ensemble Models | Improved robustness and prediction stability |

Each algorithm is evaluated independently before selecting the best-performing model for deployment.

---

# Feature Engineering

Effective feature engineering plays a critical role in fraud detection performance.

The project includes features such as:

### Transaction Features

- Transaction Amount
- Transaction Time
- Transaction Type
- Merchant Category
- Payment Method

### Customer Features

- Device Information
- New Beneficiary Status
- Transaction Frequency
- Geographic Location
- Historical Behavior

### Banking Features

- Bank Name
- Payment Channel
- Transaction Category
- Account Type

These engineered features help capture behavioral anomalies that are difficult to detect using simple rule-based systems.

---

# Model Evaluation

Each trained model is evaluated using standard classification metrics.

| Metric | Purpose |
|---------|----------|
| Accuracy | Overall prediction correctness |
| Precision | Quality of fraud predictions |
| Recall | Ability to identify fraudulent transactions |
| F1 Score | Balance between Precision and Recall |
| ROC-AUC | Model discrimination capability |

A combination of these metrics provides a more reliable assessment than accuracy alone, especially when dealing with highly imbalanced fraud datasets.

---

# Performance Overview

The system is designed to provide:

- Real-time transaction analysis
- Low-latency predictions
- Scalable inference pipeline
- High fraud recall
- Reduced false positives
- Batch transaction processing

The modular architecture allows models to be retrained and replaced without modifying the application layer.

---

# Datasets

CyberShield has been developed and evaluated using publicly available fraud detection datasets and transaction records.

Examples include:

- Credit Card Fraud Detection datasets
- Bank Account Fraud datasets
- Transaction behavior datasets
- Simulated banking transaction data

These datasets provide diverse fraud scenarios for training and evaluation.

---

# Engineering Highlights

This project demonstrates the integration of Machine Learning with software engineering principles to build a deployable fraud detection platform.

### Machine Learning

- Fraud Classification
- Ensemble Learning
- Feature Engineering
- Model Evaluation
- Probability Estimation

### Backend Development

- Flask REST APIs
- Model Serving
- Request Validation
- JSON Responses

### Frontend Development

- Interactive Streamlit Dashboard
- Data Visualization
- Real-Time Predictions
- Batch Processing

### Software Engineering

- Modular Architecture
- Separation of Concerns
- Dockerized Deployment
- Scalable Design
- API-First Development

---

# Challenges Faced

Developing a fraud detection platform presents several practical challenges.

## Class Imbalance

Fraudulent transactions represent only a small fraction of all transactions. Training reliable classifiers requires handling heavily imbalanced datasets while minimizing false negatives.

---

## Feature Engineering

Designing meaningful transaction features that effectively distinguish legitimate behavior from fraudulent activity is critical for model performance.

---

## Generalization

Fraud strategies evolve continuously. The system is designed to learn generalized behavioral patterns rather than memorizing historical fraud cases.

---

## Real-Time Prediction

Financial systems require low-latency inference. The prediction pipeline is optimized to support rapid decision-making without compromising accuracy.

---

## Deployment

Serving trained models through REST APIs while maintaining scalability and maintainability required careful architectural planning.

---

# Learning Outcomes

This project strengthened practical experience in:

- Machine Learning
- Fraud Analytics
- Financial Data Analysis
- Feature Engineering
- Ensemble Learning
- REST API Development
- Docker
- Streamlit
- Flask
- Software Architecture
- Data Visualization
- End-to-End ML Deployment

---

# Future Roadmap

CyberShield has been designed with extensibility in mind.

### Planned Enhancements

- Deep Learning-based fraud detection
- Graph Neural Networks for transaction relationship analysis
- Explainable AI (XAI) for prediction transparency
- Real-time streaming with Apache Kafka
- PostgreSQL integration
- User authentication and RBAC
- Multi-bank fraud intelligence
- Cloud deployment on AWS/Azure/GCP
- CI/CD pipeline using GitHub Actions
- Comprehensive monitoring and logging
- Fraud investigation dashboard
- LLM-powered fraud explanation assistant

---

# Skills Demonstrated

| Domain | Skills |
|----------|--------|
| Programming | Python |
| Machine Learning | Scikit-learn, XGBoost |
| Data Analysis | Pandas, NumPy |
| Backend | Flask REST APIs |
| Frontend | Streamlit |
| Deployment | Docker |
| Software Engineering | Modular Design, API Development |
| Data Visualization | Matplotlib |
| Version Control | Git, GitHub |

---

# Repository Highlights

- End-to-end Machine Learning application
- Fraud Detection using supervised learning
- RESTful API implementation
- Interactive web dashboard
- Batch transaction prediction
- Docker-ready deployment
- Modular and scalable architecture
- Financial technology (FinTech) application
- Production-oriented design

---

# Contributing

Contributions are welcome.

If you would like to improve CyberShield:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

Please ensure that new features include appropriate documentation and testing where applicable.

---

# Acknowledgements

This project builds upon several excellent open-source libraries and frameworks.

- Scikit-learn
- XGBoost
- Flask
- Streamlit
- Pandas
- NumPy
- Matplotlib
- Docker

We also acknowledge the publicly available fraud detection datasets and the open-source community that enables practical machine learning research.

---

# License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this project in accordance with the license.

---

<div align="center">

# CyberShield: Indian Fraud Detection System

**Secure Digital Transactions Through Machine Learning**

---

Developed as a machine learning solution for intelligent fraud detection across modern digital payment systems.

**Built with Python • Machine Learning • Flask • Streamlit • Docker**

---

**Developed by Utkarsh Gupta**

B.Tech Computer Science (Data Science) • AI & Machine Learning Enthusiast • Software Developer

If you found this project helpful or insightful, consider giving it a ⭐ on GitHub.

*"Building intelligent systems for safer digital financial ecosystems."*

</div>
| Primary Goal | Intelligent Fraud Detection |

---
