# 🏦 Bank Management System

A simple bank management application that allows users to manage their bank accounts, including creating accounts, depositing and withdrawing money, and updating account information.

## 🚀 Project Structure

The project is split into two main versions: a **Command Line Interface (CLI)** and a **Web Interface (GUI)**.

### 📁 File Breakdown

- **`bank.py` (The Backend Engine)**: 
  Contains the core `Bank` class. This file handles all the business logic, including:
  - Data persistence using `data.json`.
  - Account generation with unique identifiers.
  - Validation for age (18+) and PIN (4 digits).
  - Operations like deposit, withdrawal, and account updates.

- **`app.py` (The Web Interface)**: 
  A modern user interface built using **Streamlit**. It imports the `Bank` class from `bank.py` to provide a user-friendly web dashboard for all banking operations.

- **`main.py` (The CLI Interface)**: 
  A standalone implementation of the bank system that runs directly in the terminal. It provides a menu-driven experience for users who prefer a command-line approach.

- **`data.json`**: 
  The local database where user account information and balances are stored in JSON format.

## 🛠️ Installation & Usage

### Prerequisites
- Python 3.x
- Streamlit (for the web app)

```bash
pip install streamlit
```

### Running the Web App (Recommended)
```bash
streamlit run app.py
```

### Running the CLI App
```bash
python main.py
```

## ⚙️ Features
- ✅ **Account Creation**: Generate unique account numbers.
- 💰 **Money Management**: Secure deposits and withdrawals.
- 📝 **Profile Management**: Update names, emails, and PINs.
- 🗑️ **Account Closure**: Securely delete accounts.
- 💾 **Persistence**: All data is saved to a JSON file.
