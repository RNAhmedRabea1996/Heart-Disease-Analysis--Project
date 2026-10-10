# Heart-Disease-Analysis--Project
# Heart Disease Analysis

Exploratory data analysis of 917 patients to understand which factors
are associated with heart disease. Built with Python (pandas, NumPy,
Matplotlib).

## Dataset
Heart Failure Prediction Dataset (Kaggle, by fedesoriano).
12 clinical features per patient (age, sex, chest pain type, blood
pressure, cholesterol, max heart rate, etc.).
Source: [Heart Failure Prediction Dataset on Kaggle](PUT-LINK-HERE)

## Data Cleaning
- 172 patients had Cholesterol = 0, which is physiologically impossible.
  Treated as missing values.
- 152 of these 172 had heart disease, so the missing values are not
  random. Before cleaning, the data suggested patients had *lower*
  cholesterol, which was misleading.
- 1 record with RestingBP = 0 was removed.

## Key Findings
- **Sex:** heart disease rate ~63% in men vs ~26% in women (only 193
  women in the sample).
- **Age:** patients with heart disease were older on average
  (55.9 vs 50.6 years), with heavy overlap.
- **Chest pain:** asymptomatic patients (ASY) had the highest rate (79%).
- **Cholesterol:** only slightly higher in patients with heart disease.
- **Correlation:** MaxHR had the strongest relationship with heart
  disease (-0.40), followed by Age (+0.28).

## Limitations
- Hospital-referred patients, not a random population sample.
- Women are under-represented.
- Correlation does not imply causation.

## How to Run
1. Clone this repository
2. Install: `pip install pandas numpy matplotlib jupyter`
3. Run `jupyter notebook` and open `cardiac_project.ipynb`

## Author
Ahmed Rabie — cardiac nurse transitioning into healthcare data analytics.
