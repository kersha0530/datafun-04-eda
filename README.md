# datafun-04-eda

## 📌 Pro Analytics - Project Overview
## Author: Kersha Broussard (@kersha0530)
## Repository: GitHub - Pro Analytics
## Date: January 2025

## 📖 About This Project
#### Pro Analytics is a Python-based analytics project that includes:

* Data Processing & Visualization: Using pandas, numpy, matplotlib, and seaborn.
* Jupyter Notebook Support: Configured with jupyterlab, ipykernel, and ipywidgets.
* Logging & Monitoring: Integrated with loguru for easy debugging.
* Text-to-Speech Integration: Uses pyttsx3 for interactive user feedback.

**Step 1: Create a New GitHub Repository**
File: create-repo-in-github.md
Instructions:
Go to GitHub (https://github.com).
Click New Repository.
Enter repository name (pro-analytics-01).
Choose Public or Private.
Click Create Repository.
Copy the repo URL

**Step 2: Clone the Repository to Your Local Machine**
File: clone-repo-to-local.md
Command to Run in PowerShell:
powershell
Copy
Edit
cd "C:\44608 projects spring 2025"
git clone https://github.com/kersha0530/pro-analytics-01.git
cd pro-analytics-01

**Step 3: Add .gitignore and requirements.txt**
File: add-gitignore-and-requirements.md
Commands to Create & Edit Files:
powershell
Copy
Edit
# Create a .gitignore file
ni .gitignore

# Open .gitignore in VS Code to edit (or use Notepad)
code .gitignore

# Create a requirements.txt file
ni requirements.txt

# Open requirements.txt in VS Code
code requirements.txt

**Add This to requirements.txt:**

```bash```

# Essential Python packages
pip
setuptools
wheel

# Logging
loguru

# Data processing & visualization
numpy
pandas
matplotlib
seaborn

# Jupyter Notebook
jupyterlab
ipykernel
ipywidgets

# Text-to-Speech
pyttsx3

**Step 4: Add, Commit, and Push to GitHub**
File: 
git-add-commit-push.md

Commands:
```powershell```

# Add all files to Git tracking
git add .

# Commit the changes
git commit -m "Added .gitignore and requirements.txt"

# Push to GitHub
git push origin main