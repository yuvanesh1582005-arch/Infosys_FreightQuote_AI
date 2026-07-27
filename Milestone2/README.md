🚢 FreightQuote AI Platform – Milestone 2

 📌 Project Overview

**FreightQuote AI Platform – Milestone 2** is an AI-powered intelligent freight management system that extends the authentication module developed in Milestone 1 into a complete logistics decision-support platform.

This milestone integrates **Machine Learning**, **Large Language Models (LLMs)**, and **enterprise-grade security** to create a secure freight quotation system capable of predicting freight costs, identifying shipment risks, auditing carrier compliance, and generating AI-powered logistics recommendations.

The platform follows a **multi-agent architecture**, where each AI agent specializes in solving a different logistics problem while an AI Copilot combines all predictions into meaningful business insights.


🎯 Project Objectives

The primary objective of Milestone 2 is to build a secure and intelligent freight quotation platform that can:

* Secure user authentication using JWT and OTP verification
* Predict freight transportation costs
* Detect shipment delays and logistics risks
* Analyze carrier compliance
* Generate AI-powered logistics recommendations
* Provide an administrative dashboard for user management
* Improve overall logistics decision making using Machine Learning and LLMs

🚀 What This Milestone Adds

Compared to Milestone 1, this milestone introduces:

* Multi-Agent AI System
* Machine Learning Integration
* Large Language Model (LLM) Copilot
* Freight Price Prediction
* Route Delay Prediction
* Carrier Compliance Analysis
* Progressive Account Lockout
* Password Strength Verification
* OTP Rate Limiting
* Admin Dashboard
* ML Model Performance Monitoring

 🏗 System Architecture

The project follows a four-phase architecture.

# Phase 1 – Security Gateway

This is the entry point of the application.

It provides:

* User Registration
* Login Authentication
* Forgot Password
* OTP Verification using Gmail
* JWT Session Management
* Password Encryption using bcrypt
* SQLite Database Authentication

Only authenticated users can access the AI modules.

---

# Phase 2 – Intelligent Freight Agents

After successful authentication, three autonomous AI agents become available.

## Agent 1 – Dynamic Freight Pricing

Purpose:

Predicts the estimated freight transportation cost based on shipment information.

Example Inputs

* Distance
* Shipment Weight
* Port
* Fuel Cost
* Congestion Level

Output

Estimated Freight Price

Machine Learning Algorithms Compared

* Random Forest Regressor
* Gradient Boosting Regressor
* Extra Trees Regressor
* Ridge Regression
* Decision Tree Regressor
* AdaBoost Regressor
* KNeighbors Regressor

The model with the highest R² Score is selected and saved.

---

## Agent 2 – Route Delay Prediction

Purpose

Predicts whether a shipment is likely to experience delays.

Example Inputs

* Route
* Shipment Type
* Weather
* Traffic
* Port Congestion

Output

Delay Risk

Algorithms

* Random Forest Classifier
* Gradient Boosting Classifier
* Logistic Regression
* Support Vector Machine
* Extra Trees Classifier
* AdaBoost Classifier
* KNeighbors Classifier

The model with the best ROC-AUC score becomes the final model.

---

## Agent 3 – Carrier Compliance Sentinel

Purpose

Evaluates whether freight carriers satisfy logistics compliance standards.

Outputs

* Compliance Risk
* Carrier Performance
* Audit Status

Algorithms

* Gradient Boosting
* Random Forest
* Extra Trees
* Logistic Regression
* Decision Tree
* AdaBoost
* MLP Classifier

🤖 AI Copilot

One of the major additions in Milestone 2 is the AI Copilot powered by a Hugging Face LLM.

Instead of simply displaying machine learning predictions, the Copilot analyzes the outputs from all three AI agents and generates:

* Business insights
* Shipment recommendations
* Freight optimization strategies
* Risk explanations
* Structured JSON audit reports

This makes the application more than a prediction system—it becomes an AI logistics assistant.

🔒 Advanced Security Features

# JWT Authentication

Secure session management using JSON Web Tokens.

# Gmail OTP Verification

Users verify their identity using one-time passwords sent through Gmail SMTP.

# Progressive Account Lockout

To prevent brute-force attacks:

* 3 failed attempts → Account locked for 5 minutes
* 4 failed attempts → Locked for 15 minutes
* 5 failed attempts → Permanently locked until unlocked by the administrator

## OTP Resend Protection

To prevent OTP abuse:

* First resend → 60 seconds
* Second resend → 3 minutes
* Third resend → 5 minutes
* Additional requests → 1 hour cooldown

# Password Strength Checker

During registration and password reset:

Weak Password

* Less than 5 characters
* Registration blocked

Average Password

* 5–9 characters

Good Password

* 10 or more characters

Passwords are encrypted using bcrypt before being stored.

👨‍💼 Admin Dashboard

A dedicated administrator dashboard is available for users with the **Admin** role.

Administrator Features

* Add New Users
* Delete Existing Users
* Unlock Locked Accounts
* View Machine Learning Performance
* Monitor User Accounts
* Manage Roles
* View Agent Metrics

The dashboard provides complete lifecycle management of users.

 🧠 Machine Learning Pipeline

The training pipeline automatically:

1. Loads logistics datasets.
2. Cleans and preprocesses data.
3. Splits data into training and testing sets.
4. Trains multiple machine learning algorithms.
5. Evaluates model performance.
6. Selects the best-performing model.
7. Saves the trained model using Joblib.
8. Stores evaluation metrics in the SQLite database.

 📊 AI Workflow

```text
User Opens Application
          │
          ▼
Login / Registration
          │
          ▼
OTP Verification
          │
          ▼
JWT Authentication
          │
          ▼
Access Dashboard
          │
          ▼
Choose AI Module
          │
 ┌────────┼─────────┐
 │        │         │
 ▼        ▼         ▼
Pricing  Delay   Compliance
 Agent    Agent      Agent
 │         │          │
 └─────────┼──────────┘
           ▼
      AI Copilot
           ▼
Business Insights &
JSON Audit Report
           ▼
Administrator Dashboard
```

 🛠 Technologies Used

# Programming Language

* Python

# Frontend

* Streamlit
* HTML
* CSS

# Backend

* SQLite
* JWT
* bcrypt

# Artificial Intelligence

* Hugging Face Transformers
* Qwen 2.5 3B Instruct
* BitsAndBytes

# Machine Learning

* Scikit-learn
* Joblib
* Pandas
* NumPy

# Visualization

* Plotly
* Matplotlib

# Authentication

* Gmail SMTP
* OTP Verification

# Deployment

* Google Colab
* Ngrok

 📂 Project Structure

```text
Milestone2/
│
├── FreightQuote_AI_Milestone2.ipynb
├── app.py
├── auth.py
├── db.py
├── admin_dash.py
├── ui_theme.py
├── train_ml_freight.py
├── llm_engine_freight.py
├── requirements.txt
├── screenshots/
└── README.md
```

🌟 Key Features

* Secure Login System
* JWT Authentication
* Gmail OTP Verification
* Password Encryption
* Progressive Account Lockout
* OTP Rate Limiting
* Password Strength Checker
* Dynamic Freight Price Prediction
* Route Delay Prediction
* Carrier Compliance Analysis
* AI Copilot using LLM
* JSON Audit Generation
* Admin Dashboard
* ML Model Performance Monitoring
* Multi-Agent AI Architecture
* SQLite Database Integration
* Google Colab Deployment
* Ngrok Public Access

 📈 Future Enhancements

* Real-time shipment tracking
* Live weather API integration
* GPS route optimization
* Container tracking
* Voice-enabled AI logistics assistant
* Multi-language support
* Cloud deployment using Docker and Kubernetes
* Real-time logistics analytics dashboard

 📌 Conclusion

**FreightQuote AI Platform – Milestone 2** transforms a secure authentication system into a complete AI-driven logistics intelligence platform. By integrating machine learning models, a multi-agent architecture, enterprise security, and an LLM-based AI Copilot, the system provides intelligent freight pricing, route risk prediction, carrier compliance analysis, and actionable logistics recommendations. This project demonstrates the practical application of AI, ML, cybersecurity, and full-stack development in solving real-world supply chain and freight management challenges. It serves as a scalable foundation for next-generation intelligent logistics platforms. 
