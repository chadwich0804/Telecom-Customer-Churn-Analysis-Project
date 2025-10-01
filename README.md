# Telecom-Customer-Churn-Analysis-Project
A Python-based EDA of telecom customer churn, uncovering drivers like contract type (42.7% churn for month-to-month) and fiber optic usage (41.9%) to inform retention strategies.

Telecom Customer Churn Analysis

Project Overview

This repository contains a comprehensive Exploratory Data Analysis (EDA) of customer churn in a telecom dataset, designed to uncover key drivers of churn and inform retention strategies. The analysis, conducted in Python, quantifies a 26.5% churn rate and identifies critical factors such as contract type, tenure, monthly charges, and service offerings. Visualizations include histograms, bar charts, pie charts, donut charts, scatter plots, and line plots, crafted for a Wall Street-professional presentation.

Objectives





Quantify the extent of customer churn (~1,869 of 7,043 customers annually).



Identify primary drivers (e.g., 42.7% churn for month-to-month contracts, 41.9% for fiber optic users).



Provide actionable insights to reduce churn by 10-15%, potentially yielding $0.8MM in annual revenue lift.

Dataset





Source: Customer-Churn.csv (included in this repository).



Records: 7,043 customers.



Columns: 20 (after dropping customerID):





Demographics: gender, SeniorCitizen, Partner, Dependents.



Services: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies.



Billing: Contract, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges.



Target: Churn (Yes/No).



Cleaning: Converted TotalCharges to numeric, filled missing values with 0.

Requirements





Python: 3.8+



Libraries:





pandas



seaborn



matplotlib



Install dependencies:

pip install pandas seaborn matplotlib

Repository Structure





Customer-Churn.csv: Raw dataset.



eda_extended_plots.py: Python script for EDA and visualizations.



plots/: Directory for saving generated plots (create manually if needed).



README.md: This file.

Usage





Clone the Repository:

git clone https://github.com/your-username/telco-churn-analysis.git
cd telco-churn-analysis



Run the EDA Script:

python eda_extended_plots.py





Outputs: Console prints of churn rates by feature (e.g., 45.3% for electronic check) and visualizations saved as PNGs in plots/ (if plt.savefig is added).



Generate Plots for Presentation:





Modify script to include plt.savefig('plots/plot_name.png', dpi=300, bbox_inches='tight') before each plt.show() to save plots.



Use saved plots for PowerPoint slides (see recommended slide structure below).

Key Insights





Contract Type: Month-to-month contracts have a 42.7% churn rate vs. 2.9% for two-year contracts.



Tenure: Customers with <12 months tenure churn at 47.7%.



Monthly Charges: High charges (>$80) correlate with 34% churn.



Internet Service: Fiber optic users churn at 41.9%, vs. 7.4% for no internet.



Payment Method: Electronic check users churn at 45.3%, vs. ~16% for auto-payments.



Interactions: Low tenure + high charges drive >50% churn; fiber optic charges escalate rapidly in early tenure.
