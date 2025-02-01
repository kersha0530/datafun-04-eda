# datafun-04-eda

# 📊 Exploratory Data Analysis (EDA) - `datafun-04-eda`
**Author:** Kersha Broussard (@kersha0530)  
**Repository:** [GitHub - Pro Analytics](https://github.com/kersha0530/pro-analytics-01)  
**Date:** January 2025  

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on the **Iris dataset** using:
- `pandas` for data manipulation
- `matplotlib` & `seaborn` for visualization
- `numpy` for numerical analysis

This notebook is structured into **9 key sections**, each covering an essential step in EDA.

# **📊 Exploratory Data Analysis (EDA) Steps**
**1️. Imports**
We start by importing essential libraries:

```python```

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
**2️. Load the Data**
We use the built-in Iris dataset from seaborn:

```python```

iris_df: pd.DataFrame = sns.load_dataset('iris')
iris_df.head()
**3️. Initial Data Inspection**
We check the dataset’s shape, data types, and structure:

```python```

print("Dataset Shape:", iris_df.shape)
print("Data Types:\n", iris_df.dtypes)
iris_df.info()
**4️. Descriptive Statistics**
Generate statistical insights:

```python```

iris_df.describe()
**5️. Data Distribution (Numerical)**
Visualize the distribution of numerical columns:

```python```

iris_df.hist()
plt.show()
**6️. Data Distribution (Categorical)**
Analyze categorical column distributions:

```python```

iris_df['species'].value_counts()
sns.countplot(x="species", data=iris_df)
plt.show()
**7️. Feature Engineering**
We create new features for deeper analysis:

```python```

iris_df['Sepal Area'] = iris_df['sepal_length'] * iris_df['sepal_width']
**8️.  Data Visualization**
Pairplot (Feature Relationships):
python
Copy
Edit
sns.pairplot(iris_df, hue='species')
plt.show()
Scatter Plot (Sepal Length vs. Sepal Area):
```python```

scatter_plt = sns.scatterplot(data=iris_df, x="sepal_length", y="Sepal Area", hue="species")
scatter_plt.set_xlabel("Sepal Length (mm)")
scatter_plt.set_ylabel("Sepal Area (mm²)")
scatter_plt.set_title("Sepal Length vs. Sepal Area (by Species)")
plt.show()
**9️. Key Insights**
Data Shape: The dataset contains 150 rows and 5 columns.
Feature Trends: Sepal length and sepal width show a slight positive correlation.
Categorical Distribution: The dataset is evenly distributed among three species.

## **Project Setup**

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