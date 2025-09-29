PermitPulse: Predicting Construction Costs in Toronto
🌆 Why We Started This Project

This project began with a simple conversation: Why is rent in Toronto so high?
As students living in the GTA, we often talk about the struggle of housing affordability. It became clear that the issue isn’t just about demand — it’s also about how expensive it is to build housing in the first place.

That’s how PermitPulse started. We wanted to use open data to dig into Toronto’s building permits and see how construction costs are shaped by project type, location, and scale. If we could better understand these drivers, we could also better understand why Toronto housing — and rent — feels out of reach for so many people.

📌 Project Overview

PermitPulse is a data analytics project for STA302 at the University of Toronto. We analyzed the City of Toronto’s Building Permits – Cleared Permits dataset (2017–2024), which contains over 100,000 permits, and built a multiple linear regression model to predict estimated construction costs.

Predictors included:

Permit type (new building, demolition, upgrades, etc.)

Structure type (apartment, single house, multi-unit, etc.)

Ward location (geographic differences across Toronto)

Dwelling units created

Residential floor area

We applied a log-transformation to stabilize variance and improve model assumptions.

🔑 Key Findings

Permit type is the strongest driver: “New Building” permits cost nearly 37× more than baseline residential permits.

Project scale matters: More units and bigger floor areas → higher costs.

Location matters: Wards differ significantly, reflecting land values and zoning rules.

Structure type matters: Apartments and multi-unit buildings cost less per permit compared to detached houses.

The final model explained ~53% of cost variation, showing that permit data captures a substantial share of Toronto’s construction cost drivers.

🏙️ Why This Matters

Toronto’s housing affordability crisis is fueled by both demand pressures and construction costs. Our findings highlight that cost-control measures need to be tailored by project type and location.

For policymakers → insights on where housing supply bottlenecks may arise.

For developers/investors → better budgeting, risk analysis, and project planning.

For residents → a clearer picture of why rent and home prices are so high.

📂 Repository Structure
PermitPulse/
│
├── data/  
│   ├── raw_building_data.csv       # Original dataset (Cleared Building Permits 2017–2024, from City of Toronto Open Data)  
│   └── cleaned_building_data.csv   # Cleaned dataset used for analysis  
│
├── reports/  
│   ├── projectproposal.pdf  
│   ├── finalreport.pdf  
│
├── scripts/  
│   ├── pp_data_cleaning.Rmd  
│   ├── pp_final_report.Rmd  
│   ├── pp_data_cleaning.html  
│   └── pp_final_report.html  
│
└── README.md  

🚀 How to Reproduce

Download Cleared Building Permits (2017–2024) from the City of Toronto Open Data Portal

Save it as:

data/raw_building_data.csv


Run pp_data_cleaning.Rmd to clean and preprocess the dataset.

Run pp_final_report.Rmd to generate the analysis, results, and visualizations.

👉 PermitPulse connects our everyday conversations about rent to data-driven insights about Toronto’s housing costs. It shows how open data and statistical modeling can shine a light on one of the city’s biggest challenges: affordable housing.
