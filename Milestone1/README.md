# Intelligent Freight Quote Generation – Milestone 1

## 📌 Project Overview

**Intelligent Freight Quote Generation – Milestone 1** focuses on developing a secure authentication system that serves as the foundation for the Intelligent Freight Quote Generation platform. The project implements enterprise-grade user authentication with JWT session management, password encryption, OTP-based password recovery, and role-based access control using Python, Streamlit, and SQLite.

 🎯 Project Objectives

* Build a secure user authentication system
* Implement user registration and login
* Enable OTP-based password recovery
* Secure passwords using bcrypt hashing
* Manage user sessions with JWT
* Store user information securely in SQLite
* Implement role-based access control

 ✨ Key Features

* 🔐 Secure User Authentication
* 👤 User Registration
* 🔑 Secure Login
* 📧 OTP-Based Password Recovery
* 🔒 Password Encryption using bcrypt
* 🎫 JWT Session Management
* 🗄 SQLite Database Integration
* 👥 Role-Based User Access
* 🎨 Interactive Streamlit User Interface

🔄 Authentication Workflow

```text
User Registration
        │
        ▼
Password Encrypted (bcrypt)
        │
        ▼
Stored in SQLite Database
        │
        ▼
User Login
        │
        ▼
JWT Token Generated
        │
        ▼
Secure User Session
```

 🛠 Technologies Used

### Programming Language

* Python

### Frontend

* Streamlit
* HTML
* CSS

### Backend

* SQLite
* JWT
* bcrypt

### Authentication

* Gmail SMTP
* OTP Verification

### Libraries

* Streamlit
* sqlite3
* bcrypt
* PyJWT
* smtplib

📂 Project Structure

```text
Milestone1/
│── FreightQuote_AI_Milestone1.ipynb
│── app.py
│── auth.py
│── db.py
│── ui_theme.py
│── requirements.txt
└── README.md
```

🌟 Highlights

* Secure Authentication System
* JWT-Based Session Management
* Password Encryption using bcrypt
* OTP-Based Password Recovery
* SQLite Database Integration
* Role-Based Access Control
* Interactive Streamlit Interface

📌 Conclusion

**Intelligent Freight Quote Generation – Milestone 1** establishes a secure authentication foundation for the Intelligent Freight Quote Generation platform. By integrating JWT authentication, bcrypt password encryption, OTP-based password recovery, and SQLite database management, the project ensures secure user access and provides a scalable foundation for the AI-powered freight management features implemented in Milestone 2.
