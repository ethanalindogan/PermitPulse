# PermitPulse: Estimating Construction Costs from Toronto Building Permits

> A personal data science project exploring construction cost estimation in Toronto using real permit data (2017–2024), starting with regression analysis and extending into machine learning.

## 📌 Project Overview

PermitPulse investigates the key drivers of estimated construction cost using over 100,000 cleared building permits from the City of Toronto. I began with exploratory data analysis and multiple linear regression in R, and I’m extending this into a predictive machine learning project.

## 🧪 Research Question

What factors best explain the variation in estimated construction costs of Toronto building permits from 2017 to 2024?

## 🛠️ Methods and Tools

- Data Cleaning & Wrangling (R)
- Exploratory Data Analysis
- Multiple Linear Regression
- Model Diagnostics
- R Markdown for reproducibility
- (Planned) Machine Learning with Python: Random Forest, XGBoost

## 📁 Project Structure

PermitPulse/
├── data/
│ ├── cleaned_building_data.csv # Cleaned dataset
│ └── raw_building_data.csv # Source data from City of Toronto (excluded from GitHub)
│
├── analysis/
│ ├── PermitPulse_Report.html # Output from RMarkdown
│ └── PermitPulse_Model.Rmd # Source RMarkdown file
│
├── reports/
│ ├── STA302 Project Proposal.pdf
│ └── STA302 Final Report.pdf
│
├── .gitignore
├── README.md
└── requirements.txt (for ML extension - coming soon)


## 🌐 Data Source

- City of Toronto Open Data Portal:  
  Building Permits – Cleared Permits  
  https://open.toronto.ca/dataset/building-permits-cleared-permits/  
  (Saved as raw_building_data.csv)

## 📊 Key Results

- Adjusted R² = 0.449
- Permit Type and Ward significantly predict construction cost
- Diagnostics suggest log transformation may improve linear model performance

## 🔮 Future Work

- Build predictive ML models (Random Forest, XGBoost)
- Add dashboard or notebook-based exploration
- Publish findings and insights in a blog post or portfolio

## 👤 Author

Ethan Alindogan  
University of Toronto  
📫 ethan.alindogan@mail.utoronto.ca
