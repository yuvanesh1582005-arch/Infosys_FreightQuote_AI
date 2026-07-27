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

📸 1. Login Page

Description

The Login Page acts as the secure entry point to the FreightQuote AI Platform. Users authenticate using their registered email and password, which are securely stored using bcrypt hashing. After successful authentication, a JWT session token is generated to maintain a secure user session. This module also provides access to user registration and password recovery through OTP verification, ensuring that only authorized users can access the platform.
<img width="1915" height="907" alt="Screenshot 2026-07-16 193004" src="https://github.com/user-attachments/assets/abb380f1-6094-403e-aa7e-197cf38d9750" />

👤 User Dashboard

Description

The User Dashboard serves as the primary interface displayed after a successful login. It acts as the central workspace where authenticated users can access all AI-powered logistics services within the FreightQuote AI Platform. From this dashboard, users can navigate to the Dynamic Freight Pricing, Route Delay Prediction, Carrier Compliance Analysis, and AI Copilot modules to perform intelligent freight analysis and receive data-driven recommendations. The dashboard provides an intuitive and user-friendly interface, enabling users to efficiently interact with the platform while maintaining secure access through JWT authentication.
<img width="1903" height="902" alt="Screenshot 2026-07-27 185007" src="https://github.com/user-attachments/assets/51b83037-6a17-4512-b5c1-f3ac24932c03" />

💰 3. Dynamic Freight Pricing Agent

Description

The Dynamic Freight Pricing Agent predicts transportation costs using machine learning regression models. Users provide shipment details such as distance, weight, congestion level, and other logistics parameters. Multiple regression algorithms are evaluated, and the model with the highest R² score is selected to generate accurate freight cost predictions. This enables businesses to estimate transportation expenses efficiently and make informed pricing decisions.
<img width="1910" height="895" alt="Screenshot 2026-07-27 185033" src="https://github.com/user-attachments/assets/896d7fa3-74d6-400b-afa1-5584e19c39e5" />

🚚 4. Route Delay Prediction Agent

Description

The Route Delay Prediction Agent uses classification algorithms to predict the likelihood of shipment delays. It analyzes logistics data, including route information, weather conditions, traffic, and operational factors, to classify shipments into different delay-risk categories. The best-performing model is selected based on ROC-AUC evaluation, helping logistics companies proactively manage delivery risks and improve supply chain reliability.
<img width="1907" height="897" alt="Screenshot 2026-07-27 185109" src="https://github.com/user-attachments/assets/2db7e4b9-3532-494b-9716-86a5a37ae5b0" />

✅ 5. Carrier Compliance Sentinel

Description

The Carrier Compliance Sentinel evaluates freight carriers based on historical operational data and compliance metrics. It predicts carrier performance, identifies potential compliance violations, and assists logistics managers in selecting reliable transportation partners. This module supports better decision-making by reducing operational risks and improving shipment reliability.
<img width="1912" height="892" alt="Screenshot 2026-07-27 185204" src="https://github.com/user-attachments/assets/f6781724-3ec1-4086-9188-2bf667f04115" />

🤖 6. AI Copilot

Description

The AI Copilot integrates a Large Language Model (LLM) to provide intelligent logistics assistance. Instead of displaying only numerical predictions, it interprets the outputs generated by the freight pricing, route delay, and carrier compliance agents. The Copilot generates business insights, shipment recommendations, executive summaries, and structured JSON audit reports, enabling users to make informed logistics decisions through natural language interaction.
<img width="1903" height="902" alt="Screenshot 2026-07-27 185007" src="https://github.com/user-attachments/assets/4071f339-fc12-4579-b371-a1bda599b8d2" />

👨‍💼 7. Admin Dashboard

Description

The Admin Dashboard provides centralized administrative control over the FreightQuote AI Platform. Accessible only to authorized administrators, it enables user management, system monitoring, and machine learning model supervision. Administrators can monitor platform activities, view user information, and access system metrics through an intuitive interface, ensuring secure and efficient platform management.
<img width="1902" height="892" alt="Screenshot 2026-07-27 185511" src="https://github.com/user-attachments/assets/2ed4be3e-2e6d-4e1f-9615-6a1423b932a6" />

👥 8. User Management (Add / Delete / Unlock)

Description

The User Management module allows administrators to manage the complete user lifecycle. New users can be created with specific roles, inactive accounts can be removed, and locked accounts can be restored after security verification. This role-based management system ensures secure access control while simplifying administrative operations across the platform.
<img width="1902" height="892" alt="Screenshot 2026-07-27 185511" src="https://github.com/user-attachments/assets/d7dc6f0d-c590-40d8-973d-a009f881ca82" />

📊 9. Machine Learning Model Performance

Description

The Machine Learning Model Performance page displays the evaluation metrics of all trained AI models. Multiple machine learning algorithms are compared for each intelligent agent, and the best-performing model is selected based on evaluation metrics such as R² Score, RMSE, Accuracy, Precision, Recall, F1-Score, and ROC-AUC. These metrics provide transparency into the effectiveness and reliability of the predictive models.
<img width="1883" height="895" alt="Screenshot 2026-07-27 185243" src="https://github.com/user-attachments/assets/06ff20fc-67f5-4ebe-8f94-d343bcc120c8" />

🔒 10. Security Features

Description

The Security Features module demonstrates the advanced protection mechanisms implemented in the platform. It includes progressive account lockout after repeated failed login attempts, OTP resend rate limiting to prevent abuse, and a real-time password strength checker that enforces strong password policies. These features significantly enhance the security and reliability of the authentication system.
<img width="1915" height="892" alt="Screenshot 2026-07-27 185730" src="https://github.com/user-attachments/assets/d69c7f98-5228-4a28-a6a1-b89610a1130d" />

🔐 Secure Login & Progressive Account Lockout

Description:

The platform provides secure user authentication using JWT-based login, encrypted password verification, user registration, and OTP-based password recovery. To protect against brute-force attacks, it implements a Progressive Account Lockout mechanism, where the account is temporarily locked for 5 minutes after 3 consecutive failed login attempts, 15 minutes after 4 failed attempts, and permanently locked after 5 failed attempts until unlocked by an administrator.
<img width="1907" height="888" alt="Screenshot 2026-07-27 185340" src="https://github.com/user-attachments/assets/f91198d7-7369-4c12-9934-4db5436617d9" />

🔑 Password Strength Checker

Description:

The Password Strength Checker validates passwords in real time during account registration. It categorizes passwords into Weak, Average, and Good based on their length and complexity. Weak passwords (less than 5 characters) are blocked, Average passwords (5–9 characters) are accepted with a recommendation to use stronger passwords, and Good passwords (10 or more characters) are approved for secure account creation. Once validated, passwords are securely encrypted using bcrypt hashing before being stored in the database.
<img width="1866" height="896" alt="Screenshot 2026-07-27 184527" src="https://github.com/user-attachments/assets/9228890c-422d-499b-a1ac-3aaf44aeee20" />
