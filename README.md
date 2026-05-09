# 🐝 Honeybee Colony Health Prediction

Predicting whether a honeybee colony is healthy using hive inspection records and environmental weather data — built for COMP4610 (Data Mining).

---

## Project Overview

Honeybee colonies are critical to agriculture, yet health monitoring is labour-intensive and relies on manual inspection. This project applies data mining techniques to automate colony health classification from structured hive inspection and weather data, helping identify the environmental and hive-level factors most associated with colony health.

---

## Pipeline

1. Data loading & exploration (6 relational CSV files)
2. Data quality assessment
3. Data cleaning & integration
4. Post-integration cleaning
5. Noisy data handling (binning & smoothing)
6. Feature aggregation & engineering
7. Exploratory data analysis with visualizations
8. Feature encoding & normalization
9. Outlier detection
10. Dimensionality reduction (PCA + SelectKBest)
11. Classification modelling with multiple algorithms
12. Handling class imbalance with SMOTE

---

## Models Used

| Model | Library |
|---|---|
| Logistic Regression | scikit-learn |
| Decision Tree | scikit-learn |
| Random Forest | scikit-learn |
| Gradient Boosting | scikit-learn |
| AdaBoost | scikit-learn |
| K-Nearest Neighbors | scikit-learn |
| Support Vector Machine | scikit-learn |
| Naive Bayes | scikit-learn |

---

## Tech Stack

- **Language:** Python 3
- **Data wrangling:** pandas, NumPy
- **Visualization:** matplotlib, seaborn
- **Machine learning:** scikit-learn
- **Class imbalance:** imbalanced-learn (SMOTE)
- **Notebook:** Jupyter

---

## Dataset

6 relational CSV files sourced from Kaggle, covering:

| File | Description |
|---|---|
| `HCC_Inspections.csv` | Hive inspection records with health labels |
| `Hive_Information.csv` | Metadata about individual hives |
| `Apiary_Information.csv` | Apiary location details |
| `Hourly_Weather.csv` | Hourly weather readings |
| `Weather_Observations.csv` | Daily weather observations |
| `Weather_Stations.csv` | Weather station metadata |

---

## Repository Structure

```
honeybee-health-prediction/
│
├── README.md
├── Data_Mining_Project_Complete.ipynb   ← main analysis notebook
│
├── data/
│   ├── HCC_Inspections.csv
│   ├── Hive_Information.csv
│   ├── Apiary_Information.csv
│   ├── Hourly_Weather.csv
│   ├── Weather_Observations.csv
│   └── Weather_Stations.csv
│
└── docs/
    ├── COMP4610_Final_Project_Report.pdf
    └── FinalPresentation.pptx
```

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/honeybee-health-prediction.git
   cd honeybee-health-prediction
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook Data_Mining_Project_Complete.ipynb
   ```

> **Note:** The CSV dataset files must be placed in the `data/` folder before running. The notebook loads them by filename — update the file paths in Section 2 if needed.

---

## Project Report & Slides

- 📄 [Final Report](docs/COMP4610_Final_Project_Report.pdf)
- 📊 [Presentation Slides](docs/FinalPresentation(2).pptx)

---

## Course

**COMP4610 — Data Mining**
