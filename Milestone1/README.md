# 🚀 Intelligent Freight Quote Generation Using AI

## 📌 Project Overview

**Intelligent Freight Quote Generation Using AI** is a secure web application developed during my **Infosys Internship** to automate the freight quotation process using Artificial Intelligence. The application predicts freight costs based on shipment details and provides a secure platform for users to generate quotations, manage accounts, and visualize business insights.

Instead of manually calculating transportation costs, the system uses a Machine Learning model to estimate freight charges quickly and accurately, reducing human effort and improving operational efficiency.

---

# 🎯 Problem Statement

In logistics companies, freight quotations are often prepared manually by considering factors such as shipment weight, distance, transport mode, and delivery priority. This process is slow, prone to human errors, and difficult to scale when handling a large number of shipments.

To overcome these challenges, this project introduces an AI-powered solution that automatically predicts freight costs using historical shipment data while ensuring secure user authentication and a modern user experience.

---

# 💡 Solution

This project combines Machine Learning, secure authentication, and an interactive web interface into a single application.

Users can:

* Register and create an account.
* Log in securely using encrypted credentials.
* Recover forgotten passwords through OTP email verification or security questions.
* Enter shipment details.
* Generate AI-based freight cost predictions.
* View business analytics through interactive dashboards.

---

# ✨ Key Features

### 🔐 Secure Authentication System

A complete authentication module was developed to ensure secure access.

It includes:

* User Registration
* Secure Login
* Password Hashing using **bcrypt**
* JWT Token Authentication
* Forgot Password
* OTP Email Verification
* Security Question Verification
* Session Management
* Token Expiration

---

### 🤖 AI-Based Freight Cost Prediction

The core functionality of this project is predicting freight costs using Machine Learning.

The model analyzes shipment information such as:

* Shipment Weight
* Shipment Volume
* Distance
* Transportation Mode
* Pickup Location
* Destination
* Delivery Priority

After processing these values, the trained Random Forest model predicts an estimated freight cost within seconds.

---

### 📊 Interactive Dashboard

A professional dashboard was created using **Streamlit** and **Plotly**.

The dashboard displays:

* Freight predictions
* System status
* User information
* Interactive charts
* Performance indicators
* Business analytics

The UI follows a modern **Nebula Control Tower** design with animated particle backgrounds, gradient themes, responsive cards, and clean navigation.

---

# 🛠 Technologies Used

| Technology   | Purpose                             |
| ------------ | ----------------------------------- |
| Python       | Core programming language           |
| Streamlit    | Web application development         |
| HTML & CSS   | User Interface customization        |
| Plotly       | Interactive charts and dashboards   |
| SQLite       | Local database storage              |
| Pandas       | Data preprocessing                  |
| NumPy        | Numerical computations              |
| Scikit-learn | Machine Learning                    |
| JWT          | Secure user authentication          |
| bcrypt       | Password encryption                 |
| SMTP         | Sending OTP emails                  |
| Pyngrok      | Public deployment from Google Colab |

---

# 🤖 Machine Learning

The application uses the **Random Forest Regressor** algorithm.

### Why Random Forest?

Random Forest was selected because it:

* Produces high prediction accuracy
* Handles nonlinear relationships
* Reduces overfitting
* Works well with structured logistics data
* Is reliable for regression problems

The model was trained using historical freight data after performing preprocessing and feature engineering.

---

# 📂 Data Preprocessing

Before training the model, the dataset was cleaned by:

* Removing duplicate records
* Handling missing values
* Encoding categorical features
* Selecting important features
* Splitting the dataset into training and testing sets

These preprocessing steps improve prediction accuracy and model reliability.

---

# 📈 Data Visualization

To understand the dataset better, multiple visualizations were created using Plotly, including:

* Shipment distribution
* Transport mode analysis
* Correlation heatmaps
* Feature importance
* Freight cost distribution
* Performance indicators

These visualizations help analyze trends and improve business decisions.

---

# 🔐 Security Implementation

Security was one of the major focuses of this project.

### Password Hashing (bcrypt)

Passwords are never stored as plain text.

Instead, bcrypt converts passwords into encrypted hashes before storing them in the database.

This protects user credentials even if the database is compromised.

---

### JSON Web Token (JWT)

JWT is used to authenticate users after login.

Instead of checking the database for every request, a secure token is generated and verified.

Benefits include:

* Faster authentication
* Secure user sessions
* Token expiration
* Protection against unauthorized access

---

### OTP Email Verification

If users forget their password, they can request an OTP.

The system:

* Generates a random 6-digit OTP.
* Sends it through Gmail SMTP.
* Validates the OTP.
* Allows password reset only after successful verification.

OTP expires automatically after 5 minutes to improve security.

---

### Security Questions

As an alternative recovery method, users can reset their password by answering their predefined security question.

---

# 💾 Database

SQLite is used as the backend database.

It stores:

* User details
* Email addresses
* Encrypted passwords
* Security questions
* Password reset information

SQLite was selected because it is lightweight, easy to configure, and suitable for small to medium-sized applications.

---

# 📧 Email Integration

SMTP is integrated for sending verification emails.

The system automatically sends:

* OTP verification codes
* Password reset notifications

Professional HTML email templates were designed to improve the user experience.

---

# 🌐 Deployment

The application was developed and tested in **Google Colab**.

Since Streamlit applications cannot be accessed directly from Colab, **Pyngrok** was used to generate a public URL, allowing anyone to access the application through a browser.

---

# 🔄 Project Workflow

1. User registers a new account.
2. Password is encrypted using bcrypt.
3. User logs in securely.
4. JWT token is generated.
5. User enters shipment details.
6. Data is preprocessed.
7. Random Forest predicts the freight cost.
8. Prediction is displayed on the dashboard.
9. Users can recover forgotten passwords using OTP or security questions.

---

# 📚 What I Learned

This project provided practical experience in:

* Machine Learning
* Data preprocessing
* AI model development
* Streamlit web application development
* SQLite database management
* Secure authentication using JWT
* Password encryption with bcrypt
* Email integration using SMTP
* Dashboard development using Plotly
* Deployment using Pyngrok
* Git and GitHub version control
* End-to-end AI application development

---

# 🚀 Future Improvements

Future enhancements planned for this project include:

* Cloud deployment on AWS or Azure
* Real-time logistics API integration
* Live shipment tracking
* PDF freight quotation generation
* Role-based access control
* Mobile application support
* Multi-language interface
* Advanced AI models for improved prediction accuracy
* Customer support chatbot using Generative AI

---

# ✅ Conclusion

The **Intelligent Freight Quote Generation Using AI** project demonstrates how Artificial Intelligence can modernize logistics operations by automating freight quotation generation. By combining Machine Learning, secure authentication, interactive dashboards, and a responsive web interface, the application delivers faster, more accurate, and secure freight cost estimation. This project strengthened my practical knowledge of AI, Machine Learning, web development, cybersecurity, database management, and software deployment while solving a real-world logistics problem.

🔐 1. Login Page

Description:
Secure authentication page where registered users can log in using their email and password. The system validates credentials using JWT authentication and bcrypt password hashing to ensure secure access to the application.
<img width="1915" height="907" alt="Screenshot 2026-07-16 193004" src="https://github.com/user-attachments/assets/eded30ab-2e4f-423a-8adc-656d895530ff" />

📝 2. Create Account

Description:
User registration page that allows new users to create an account by providing their personal details, email, password, and security question. Passwords are securely encrypted before being stored in the database.
<img width="1911" height="907" alt="Screenshot 2026-07-16 193019" src="https://github.com/user-attachments/assets/91c74e4d-459a-485b-bbd3-85f444b38cff" />

🔑 3. Forgot Password

Description:
Password recovery page that provides two secure recovery options: resetting the password using a registered security question or receiving a One-Time Password (OTP) via email.
<img width="1916" height="910" alt="Screenshot 2026-07-16 192941" src="https://github.com/user-attachments/assets/57986345-1661-4409-89a9-b2d612f4273a" />

📧 4. OTP Verification

Description:
Verification page where users enter the OTP received through email. The OTP is securely validated and expires after a limited time to prevent unauthorized access.
<img width="1916" height="906" alt="Screenshot 2026-07-16 193125" src="https://github.com/user-attachments/assets/4c8086ed-6a7c-4f02-8607-6da57b365273" />

🔒 5. Reset Password

Description:
Allows users to create a new password after successful verification. The application enforces password strength requirements and securely updates the encrypted password in the database.
<img width="1917" height="902" alt="Screenshot 2026-07-16 193837" src="https://github.com/user-attachments/assets/16232052-ff49-4d20-a3bc-d16d0d2c20a0" />

📊 6. Analytics Dashboard

Description:
Interactive dashboard built with Plotly to visualize shipment data, business insights, and system performance through dynamic charts and graphs, helping users make informed decisions.
<img width="1916" height="902" alt="Screenshot 2026-07-16 193052" src="https://github.com/user-attachments/assets/1336b338-32fd-45af-a691-97a5ade90850" />
