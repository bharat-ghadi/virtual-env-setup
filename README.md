
# Project Virtual Environment Setup

This README provides detailed instructions to create and activate a Python 3.9 virtual environment for the project.

---

## 📋 Prerequisites

- **Python 3.9**: Make sure Python 3.9 is installed on your system. You can verify this by listing installed Python versions:
  ```bash
  py -0
  ```

---

## 🚀 Steps to Set Up the Virtual Environment

1. ### Navigate to Your Desired Directory
   Open your terminal and navigate to the directory where you want to set up the virtual environment.

2. ### Create the Virtual Environment
   Use Python 3.9 to create a new virtual environment:
   ```bash
   py -3.9 -m venv D:\Virtual_Environments\env39
   ```
   #### Generic Command Format:
   ```
   py <python version (e.g., 3.9)> -m venv <env path (e.g., D:\Virtual_Environments\env39)>
   ```
   This command will create a virtual environment named `env39` in `D:\Virtual_Environments`.

3. ### Activate the Virtual Environment
   After creating the environment, activate it based on your shell type:

   - **For Command Prompt**:
     ```cmd
     D:\Virtual_Environments\env39\Scripts\activate.bat
     ```

   - **For PowerShell**:
     ```powershell
     D:\Virtual_Environments\env39\Scripts\Activate.ps1
     ```

4. ### Confirm the Python Version
   Verify that your virtual environment is using Python 3.9 by running:
   ```bash
   python --version
   ```
   The output should display Python 3.9.x.

5. ### Install Project Dependencies
   If your project has dependencies, install them by running:
   ```bash
   pip install -r requirements.txt
   ```

---

## ❌ Deactivating the Virtual Environment

To exit the virtual environment, simply type:
```bash
deactivate
```

---

## 📄 Notes

- **Execution Policy for PowerShell**: If you encounter an execution policy error when activating in PowerShell, you may need to adjust the policy:
  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```

- **Requirements File**: Ensure a `requirements.txt` file is available in your project directory to install all necessary dependencies.

---
