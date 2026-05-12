# 🚀 Her Safe Path - Project Setup & Execution Guide

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python)
![Django](https://img.shields.io/badge/Django-Framework-green?style=for-the-badge\&logo=django)
![SQLite](https://img.shields.io/badge/SQLite-Database-lightgrey?style=for-the-badge\&logo=sqlite)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

---

# 📌 Project Overview

**Her Safe Path** is a women safety and emergency assistance web application developed using Django.
The platform helps users send emergency alerts and location details to trusted contacts during unsafe situations.

The application includes:

* 🔐 User Authentication
* 📍 Emergency Location Sharing
* 📧 Email Alert System
* 📱 Trusted Contacts Management
* 🆘 Panic / Emergency Button
* 🖥️ Responsive User Interface

---

# 🛠️ Tech Stack

## Frontend

* HTML5
* CSS3
* Bootstrap
* JavaScript

## Backend

* Python
* Django

## Database

* SQLite3

---

# 📂 Project Structure

```bash
her-safe-path/
│
├── main_app/              # Main Django application
├── Documentation/         # Project documentation files
├── templates/             # HTML templates
├── static/                # CSS, JS, images
├── db.sqlite3             # SQLite database
├── manage.py              # Django project manager
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation
```

---

# ⚙️ Prerequisites

Before running the project, make sure the following software is installed:

| Software              | Version |
| --------------------- | ------- |
| Python                | 3.8+    |
| Git                   | Latest  |
| pip                   | Latest  |
| Virtualenv (Optional) | Latest  |

---

# 📥 Installation Guide

## Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/her-safe-path.git
```

---

## Step 2: Navigate to the Project Directory

```bash
cd her-safe-path
```

---

## Step 3: Create Virtual Environment (Recommended)

### For Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### For Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## Step 4: Install Project Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment & Configuration Setup

Before running the project, configure the required settings.

## Update Email Configuration

Modify the following files with your email credentials and settings:

```bash
main_app/mail.py
```

and

```bash
settings.py
```

### Example Email Configuration

```python
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_HOST_USER = 'your-email@gmail.com'
EMAIL_HOST_PASSWORD = 'your-password'
EMAIL_USE_TLS = True
```

> ⚠️ Never upload your real passwords or secret keys to GitHub.

---

# 🗄️ Database Setup

## Step 5: Make Migrations

```bash
python manage.py makemigrations
```

---

## Step 6: Apply Migrations

```bash
python manage.py migrate
```

---

# 👤 Create Admin User

## Step 7: Create Superuser

```bash
python manage.py createsuperuser
```

Enter:

* Username
* Email
* Password

---

# ▶️ Run the Project

## Step 8: Start Development Server

```bash
python manage.py runserver
```

---

# 🌐 Access the Application

Open your browser and visit:

```bash
http://127.0.0.1:8000/
```

Admin Panel:

```bash
http://127.0.0.1:8000/admin
```

---

# 🧪 Common Development Commands

## Run Server

```bash
python manage.py runserver
```

## Create Migrations

```bash
python manage.py makemigrations
```

## Apply Migrations

```bash
python manage.py migrate
```

## Create Admin User

```bash
python manage.py createsuperuser
```

## Collect Static Files

```bash
python manage.py collectstatic
```

---

# 🐞 Troubleshooting Guide

## Issue: ModuleNotFoundError

### Solution

Install dependencies again:

```bash
pip install -r requirements.txt
```

---

## Issue: Port Already in Use

### Solution

Run the server on another port:

```bash
python manage.py runserver 8001
```

---

## Issue: Database Errors

### Solution

Delete migration files (except `__init__.py`) and run:

```bash
python manage.py makemigrations
python manage.py migrate
```

---

# 📦 Recommended GitHub Upload Structure

Before uploading to GitHub:

✅ Include:

* Source Code
* requirements.txt
* README.md
* Documentation
* Static Assets

❌ Exclude:

* venv/
* **pycache**/
* .env
* Personal Credentials
* IDE files

---

# 🔒 Security Best Practices

* Use environment variables for secrets.
* Never expose API keys.
* Use `.gitignore` properly.
* Keep dependencies updated.
* Validate user input.

---

# 📄 Sample .gitignore

```gitignore
venv/
__pycache__/
*.pyc
.env
db.sqlite3
.idea/
.vscode/
```

---

# 🤝 Contribution Guidelines

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Commit your changes
5. Push to your branch
6. Create a Pull Request

---

# 📘 Generic Project Execution Manual (Reusable for Any Project)

This section can be reused for almost any Python/Django project.

## Standard Workflow

```bash
# Clone Repository
git clone <repository-url>

# Enter Project Folder
cd <project-folder>

# Create Virtual Environment
python -m venv venv

# Activate Environment
venv\Scripts\activate

# Install Dependencies
pip install -r requirements.txt

# Database Setup
python manage.py makemigrations
python manage.py migrate

# Run Project
python manage.py runserver
```

---

# 📸 Suggested README Sections for Future Projects

You can reuse this structure for future GitHub projects:

* Project Title
* Project Overview
* Features
* Tech Stack
* Installation Guide
* Configuration Setup
* Execution Steps
* API Documentation
* Screenshots
* Folder Structure
* Troubleshooting
* Contribution Guide
* License

---

# 📃 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

Developed by **Ajinkya Akole**

GitHub: [https://github.com/your-github-username](https://github.com/your-github-username)

---

# ⭐ Support

If you like this project:

* Give it a ⭐ on GitHub
* Share it with others
* Contribute to improve it

---

# 🎯 Final Notes

This README is designed to:

✅ Help recruiters understand your project quickly
✅ Make project setup easy for contributors
✅ Improve professionalism of your GitHub repository
✅ Provide reusable execution steps for future projects

---
