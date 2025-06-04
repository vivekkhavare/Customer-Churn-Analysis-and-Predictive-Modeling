# Customer Churn Analysis and Predictive Modeling 📊🚀

## Project Overview
This project focuses on analyzing customer churn for a telecommunications company, leveraging a dataset of **7,043 customer records** to uncover key churn drivers and predict churn likelihood. By combining **exploratory data analysis (EDA)**, **machine learning**, and **data visualization**, the project delivers actionable insights and strategic recommendations to reduce churn by **15-40%**. An interactive **Power BI dashboard** visualizes churn patterns, enabling stakeholders to make data-driven retention decisions.

This project showcases my expertise in **predictive modeling**, **data analytics**, and **business intelligence**, with a focus on transforming raw data into measurable business impact. It was developed using **Python** in Google Colab and **Power BI** for visualization, with outputs saved for seamless integration.

---

## Table of Contents
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Tools and Technologies](#tools-and-technologies)
- [Methodology](#methodology)
- [Results and Insights](#results-and-insights)
- [Power BI Dashboard](#power-bi-dashboard)
- [Installation and Setup](#installation-and-setup)
- [Contact](#contact)

---

## Objectives
- Identify key factors driving customer churn (e.g., tenure, contract type, monthly charges).
- Build a predictive model to classify customers likely to churn with high accuracy.
- Develop an interactive Power BI dashboard to visualize churn patterns and insights.
- Propose data-driven retention strategies to reduce churn and enhance business outcomes.

---

## Dataset
- **Source**: Telco Customer Churn dataset (`customer_churn_telecom_services.csv`).
- **Size**: 7,043 customer records.
- **Features**: 21 columns, including demographic data (e.g., gender, tenure), service usage (e.g., InternetService, OnlineSecurity), billing details (e.g., MonthlyCharges, TotalCharges), and churn status (26.54% churn rate).
- **Challenges**: Handled class imbalance using SMOTE and imputed 11 missing values in `TotalCharges` with median values.

---

## Tools and Technologies
- **Programming**: Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Machine Learning**: Random Forest, SMOTE for class imbalance
- **Visualization**: Power BI
- **Database**: MySQL (for data preprocessing and storage)
- **Environment**: Google Colab
- **Outputs**: Saved model (`churn_model.pkl`), predictions (`test_predictions.csv`), visualizations (e.g., `churn_distribution.png`)

---

## Methodology
1. **Data Preprocessing**:
   - Loaded dataset using Pandas in Google Colab.
   - Handled missing values in `TotalCharges` using median imputation.
   - Encoded categorical variables (e.g., `Contract`, `PaymentMethod`) using one-hot encoding.
   - Created two novel features: `TenureGroup` (binning tenure) and `TotalServices` (count of services used).
   - Applied SMOTE to address class imbalance (26.54% churn rate).

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed churn distribution and correlations using Seaborn and Matplotlib.
   - Identified key predictors: short tenure (<12 months), month-to-month contracts, and high monthly charges.

3. **Predictive Modeling**:
   - Trained a Random Forest model, achieving an **AUC-ROC score of 0.84**.
   - Evaluated model performance using accuracy, precision, recall, and F1-score.
   - Saved the trained model as `churn_model.pkl` for deployment.

4. **Data Visualization**:
   - Imported processed data (`test_predictions.csv`) into Power BI.
   - Designed a three-page interactive dashboard with visuals like bar charts, treemaps, and donut charts to showcase churn patterns, demographics, and predictive outcomes.

5. **Strategic Recommendations**:
   - Proposed long-term contract incentives and service bundling (e.g., OnlineSecurity, StreamingTV) to reduce churn by **15-40%**.

---

## Results and Insights
- **Model Performance**: Random Forest model achieved an **AUC-ROC of 0.84**, accurately identifying high-risk customers.
- **Key Insights**:
  - Customers with <12 months tenure are **3x more likely to churn**.
  - Month-to-month contracts have a **40% higher churn rate** than long-term contracts.
  - High monthly charges (>₹5,000) correlate with increased churn.
- **Business Impact**: Proposed retention strategies (e.g., contract incentives, service bundling) are projected to reduce churn by **15-40%**, potentially saving millions in revenue.
- **Visualization**: The Power BI dashboard provides interactive insights into churn drivers, enabling stakeholders to prioritize retention efforts.

---

## Power BI Dashboard
The dashboard consists of three interactive pages:
1. **Overview Page**: Displays churn rate, customer demographics, and service usage (e.g., bar chart of churn by contract type).
2. **Predictive Insights Page**: Visualizes model predictions, highlighting high-risk customers (e.g., treemap of churn probability by tenure).
3. **Actionable Recommendations Page**: Summarizes retention strategies with visuals like donut charts for service bundling impact.

**Screenshots**: Available in the `visualizations/` folder (e.g., `churn_distribution.png`).

---

## Installation and Setup
To replicate this project, ensure you have the following:
- **Python 3.8+** with libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `imblearn`.
- **Power BI Desktop** (free download from Microsoft).
- **MySQL** for data storage (optional).
- **Google Colab** for running the code (or local Jupyter Notebook).
- Dataset: `customer_churn_telecom_services.csv` (available in the repository).

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/vivekkhavare/customer-churn-analysis.git


### Contact
I’m passionate about leveraging data analytics to solve real-world problems! Connect with me:

**LinkedIn**: Vivek Khavare
**Email**: vivekkhavare733@gmail.com
**Portfolio**: vivekkhavare.github.io
Feel free to star this repository or reach out to discuss the project! 🌟

