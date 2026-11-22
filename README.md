# Financial Fraud Detection — Data Preprocessing & Exploratory Analysis

A **team-based academic project** for the *Data Collection and Preprocessing* course at Umm Al-Qura University (April–May 2026). We used Python in Google Colab to assess, clean, transform, and explore financial transaction data, with the goal of preparing features for future fraud-detection modeling.

> **Scope:** This project focuses on data preprocessing, exploratory analysis, and feature selection. It does **not** present a trained and evaluated final fraud prediction model.

## Dataset

- **Source:** [Fraud Detection Transactions Dataset on Kaggle](https://www.kaggle.com/datasets/barkataliarbab/fraud-detection-transactions)
- **Size:** 50,000 transactions and 21 original columns.
- **Target:** `Fraud_Label` (fraudulent vs. non-fraudulent transaction).
- **Files:** `Fraud Detection Transactions Dataset.csv` is the original dataset. `Fake Fraud dataset.csv` is a modified practice copy used to demonstrate missing-value handling; the original dataset contained no missing values.

## Tools & Libraries

Python · Google Colab · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · category_encoders

## Project Workflow

1. **Data loading and inspection:** Loaded transaction records and examined columns, data types, and summary statistics.
2. **Data quality assessment:** Checked missing values, duplicate records, inconsistent categories, invalid values, and outliers.
3. **Data cleaning and EDA:** Practiced mean, median, and mode imputation on the modified dataset; examined distributions and relationships with visualizations.
4. **Outlier handling:** Used IQR and boxplots to identify extreme transaction amounts. Retained potentially meaningful transactions and applied a `log(x + 1)` transformation to reduce skewness.
5. **Transformation and feature engineering:** Compared Min-Max, Standard, and Robust scaling; explored label, one-hot, and binary encoding; derived transaction time features.
6. **Feature selection and dimensionality reduction:** Explored correlation analysis, Recursive Feature Elimination (RFE) with Logistic Regression, and PCA.
7. **Final analysis:** Summarized fraud patterns and documented conclusions and limitations.

## Key Findings

- Approximately **32%** of transactions in the dataset were labeled fraudulent.
- Fraudulent transactions tended to have **higher risk scores** and **more failed transaction attempts**.
- Weekend and weekday fraud rates were **similar** in this dataset.
- The report's selected compact dataset contained **50,000 rows and four columns**: `Failed_Transaction_Count_7d`, `Risk_Score`, `Is_Weekend`, and `Fraud_Label`.

These are observations from the analyzed dataset, not claims about real-world fraud detection performance.

## Teamwork & Contributions

This project was completed by a **two-member student team** with divided implementation responsibilities.

**Repository owner's contributions:**
- Data loading and inspection
- Data quality assessment
- Data cleaning and exploratory data analysis (EDA)
- Outlier detection and handling
- Writing, organizing, and finalizing the full technical report, including findings and conclusions

**Teammate's contributions:** The remaining implementation sections, including later transformation and feature-related tasks.

## How to Run

1. Open the `.ipynb` notebook in **Google Colab**.
2. Upload both CSV files into the Colab session's working directory, keeping their filenames unchanged.
3. Run the notebook cells in order. The notebook includes a `pip install category_encoders` command for its additional dependency.
4. If the Colab runtime resets, upload the CSV files again before rerunning.

**Note:** The repository notebook currently has a filename ending in `(1).ipynb`; open that file unless it is renamed later.

## Project Report

The full academic report documents the methodology, visualizations, results, conclusions, and limitations. A privacy-reviewed team-report PDF can be linked here once uploaded to this repository.

## Academic Context

- **Course:** Data Collection and Preprocessing
- **University:** Umm Al-Qura University, Department of Data Science
- **Project period:** April 24 – May 1, 2026
- **Type:** Team academic project (2 students)
