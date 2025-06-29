
# Secure Login System with User Role Management 🛡️

## 📌 Objective
To develop a secure web-based login system that implements user **authentication**, **authorization**, and **role-based access control (RBAC)** using Python (Flask) and MongoDB. This project demonstrates essential cybersecurity principles including password hashing, session management, CAPTCHA protection, and access control.

---

## 📂 Table of Contents

1. [Project Setup](#1-project-setup)
2. [Frontend Overview](#2-frontend-overview)
3. [Backend Structure](#3-backend-structure)
4. [Core Features](#4-core-features)
5. [Security Enhancements](#5-security-enhancements)
6. [Screenshots](#6-screenshots)
7. [Installation and Usage](#7-installation-and-usage)
8. [Challenges & Solutions](#8-challenges--solutions)
9. [Final Submission](#9-final-submission)

---

## ✅ 1. Project Setup

- IDE: Visual Studio Code
- Backend: Flask (Python)
- Database: MongoDB
- Version Control: Git + GitHub

---

## 🎨 2. Frontend Overview

The frontend consists of multiple HTML pages with role-specific and secure workflow features.

### Pages Included

| Page Name               | Description                                                             |
|-------------------------|-------------------------------------------------------------------------|
| `index.html`            | Landing or welcome page                                                 |
| `login.html`            | Login form for users                                                    |
| `register.html`         | Registration page with role selection (Admin/User)                      |
| `admin_dashboard.html`  | Dashboard for Admin to view/manage users                                |
| `user_dashboard.html`   | Dashboard for regular Users                                             |
| `forgot_password.html`  | Form to initiate password recovery                                      |
| `security_question.html`| Step 2 in password recovery – verify user identity                      |
| `verify_otp.html`       | Enter OTP sent to registered email                                      |
| `reset_password.html`   | Set a new password after OTP verification                               |

### Features

- Responsive layout using CSS
- Frontend validation for email and password
- Role-based navigation

---

## 🧠 3. Backend Structure

- **Framework:** Flask
- **Database:** MongoDB
- **Libraries Used:** `flask`, `flask_mail`, `pymongo`, `bcrypt`, `itsdangerous`, `requests`
- **Folder Structure:**
  ```
  project/
  ├── static/
  ├── templates/
  ├── app.py
  ├── config.py
  └── README.md
  ```

---

## 🔐 4. Core Features

### ✅ User Registration
- Password hashing with `bcrypt`
- Role selection
- Input validation

### ✅ User Login
- Session management
- Email and password verification
- Role-based redirection

### ✅ RBAC (Role-Based Access Control)
- Admin can view all users
- Users have limited dashboard access
- Secure routing using decorators

---

## 🛡️ 5. Security Enhancements

- Input sanitization
- CAPTCHA (optional)
- Account lockout after 3 failed attempts
- Secure session cookies

---

## 📷 6. Screenshots

> 📁 Store all screenshots inside a `screenshots/` folder. Suggested filenames below:

| Page/File Name           | Screenshot Description                     | File Name Suggestion               |
|--------------------------|---------------------------------------------|------------------------------------|
| `index.html`             | Landing or home page                        | `screenshots/index.png`            |
| `login.html`             | Login form                                  | `screenshots/login.png`            |
| `register.html`          | Registration form with role selection       | `screenshots/register.png`         |
| `admin_dashboard.html`   | Admin dashboard showing users               | `screenshots/admin_dashboard.png`  |
| `user_dashboard.html`    | Basic user dashboard                        | `screenshots/user_dashboard.png`   |
| `forgot_password.html`   | Forgot password entry page                  | `screenshots/forgot_password.png`  |
| `security_question.html` | Answer security question page               | `screenshots/security_question.png`|
| `verify_otp.html`        | OTP verification page                       | `screenshots/verify_otp.png`       |
| `reset_password.html`    | New password input form                     | `screenshots/reset_password.png`   |

---

## ⚙️ 7. Installation and Usage

### 🔧 Prerequisites
- Python 3.8+
- MongoDB
- Git

### 🚀 Setup Instructions

```bash
# Clone the repository
git clone https://github.com/<your-username>/secure-login-system.git
cd secure-login-system

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

Update `config.py` with your MongoDB URI.

---

## 🚧 8. Challenges & Solutions

| Challenge                           | Solution                                |
|------------------------------------|-----------------------------------------|
| Secure password storage            | Used `bcrypt` hashing                   |
| Brute-force protection             | CAPTCHA and account lockout             |
| Role-based redirection             | Used Flask decorators and session       |
| Form validation                    | Frontend + backend checks               |

---

## 📝 9. Final Submission

- ✅ All core features implemented
- ✅ Pages added: login, register, dashboard, forgot/reset password
- ✅ Role-based navigation working
- ✅ Screenshots placed in `screenshots/` folder
- ✅ Code structured and documented

---

## 📎 GitHub Repository

> 🔗 [https://github.com/<your-username>/secure-login-system](https://github.com/<your-username>/secure-login-system)

---

## 📧 Contact

For queries, raise an issue or contact: **[your.email@example.com](mailto:your.email@example.com)**

---
