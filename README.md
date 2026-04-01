# Patient Readmission & Financial Risk Analysis

📈 Business Overview
In the modern healthcare landscape, hospital readmissions are a multi-billion dollar challenge. Under value-based care models, high readmission rates lead to significant government penalties and operational strain.

This project provides a data-driven solution to identify high-risk patient cohorts and quantify the potential financial impact of targeted interventions. By predicting risk before discharge, healthcare providers can optimize resource allocation and improve patient outcomes.

💰 Key Business Impact
- Identified $60.11M in potential financial liability from high-risk patients.
- Segmented $36.9M of risk within the Medicare population, highlighting a key area for policy intervention.
- Discovered Seasonal Trends: Significant spikes in readmissions during December and January, suggesting a need for increased seasonal staffing.

🛠️ Tech Stack
- Data Cleaning & Engineering: Python (Pandas, NumPy)
- Exploratory Data Analysis: Python (Seaborn, Matplotlib)
- Business Intelligence: Power BI (DAX, Data Modeling)
- Environment: Jupyter Notebook

📂 Project Structure
raw_data/
-- hospital_readmission_dataset.csv

python_analysis/
-- patient_readmission_analysis_v1.ipynb
-- processed_healthcare_data_2026.csv

PowerBI_Dashboard/
-- Patient Readmission & Financial Risk Dashboard.pbix

🧪 Data Engineering & Methodology
Before visualization, the raw data underwent extensive "Business Logic" transformation in Python:
- Risk Categorization: Developed a risk-stratification model labeling patients as Low, Medium, or High Risk based on clinical scores.
- Financial Modeling: Engineered a Potential Savings metric (Risk Score * Average Readmission Cost of $15k) to translate clinical data into business metrics.
- Age & Clinical Grouping: Binned ages into cohorts (e.g., 66-80) and categorized comorbidity severity to find hidden correlations.
- Time-Series Prep: Extracted and indexed admission months to ensure chronological trend analysis.

📊 Dashboard Insights
The final Power BI dashboard serves as a decision-support tool for Hospital Administrators:
- Executive Summary: High-level KPIs showing a 77.29% Readmission Rate and an average risk score of 0.78.
- Risk Profile: A breakdown showing that 55.7% of the current patient population falls into the "High Risk" category.
- Diagnosis Breakdown: Identification of Diabetes and Hypertension as the primary drivers of readmission volume.
- Regional Analysis: The South Region holds the highest financial risk at $15.0M, indicating where to launch the first pilot intervention program.

📸 PowerBI Dashboard:

<img width="1168" height="658" alt="image" src="https://github.com/user-attachments/assets/92d5c8a2-4bd8-46d3-be8b-3ecf3fee8ec8" />


🚀 How to Use
- Python: Open patient_readmission_analysis_v1.ipynb to view the data transformation pipeline.
- Power BI: Load the .pbix file to interact with the dashboard. (Note: Ensure the data source points to the processed_healthcare_data_2026.csv).
