# Student Performance Prediction

A machine learning project to predict secondary school students' final grades (G3) using academic and socio-demographic features.

---

## About

This project compares multiple ML regression models to find the best predictor of student performance. The aim is to help educators identify at-risk students and take timely action.

---

## Dataset

- **Source:** [UCI ML Repository — Student Performance](https://archive.ics.uci.edu/dataset/320/student+performance)
- **File:** `student-por.csv`
- **Size:** 649 records, 33 variables
- **Target:** `G3` — final grade (0–20)

---

## What We Did

1. Checked for null values — none found
2. Dropped `G1` and `G2` (intermediate grades) to avoid data leakage
3. Encoded categorical variables using binary mapping and one-hot encoding
4. Removed multicollinear features using VIF (threshold > 3.5)
5. Ran EDA — histograms, heatmap, scatter plots, box plots, pie charts
6. Trained and evaluated 7 models across 4 train-test splits

---

## Models Compared

- Linear Regression
- K-Nearest Neighbours (KNN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- XGBoost
- AdaBoost
- Artificial Neural Network (ANN)

---

## Results (80-20 split, after VIF correction)

| Model | MAE | R² |
|---|---|---|
| AdaBoost | **1.767** | 0.206 |
| SVM | 1.735 | 0.145 |
| Random Forest | 1.821 | 0.155 |
| Linear Regression | 1.712 | 0.177 |
| ANN (75-25 split) | 1.884 | — |
| KNN | 1.955 | 0.006 |
| Decision Tree | 2.512 | -0.608 |

**AdaBoost gave the best overall performance** with the lowest MAE after VIF correction on the 80-20 split.

---

## Key Findings

- Study time and parental education level are the strongest predictors of final grade
- More absences and past failures correlate with lower grades
- Social factors like going out frequently and alcohol consumption negatively affect performance
- Decision Tree overfitted badly; ensemble methods worked best

---

## Tech Stack

`pandas` · `numpy` · `matplotlib` · `seaborn` · `scikit-learn` · `xgboost` · `tensorflow` · `statsmodels`

---

## Getting Started

```bash
git clone https://github.com/<your-username>/student-performance-prediction.git
cd student-performance-prediction
pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow statsmodels
jupyter notebook Regression_Project_HDS_2024__Group_10_UNP.ipynb
```

> Originally built on Google Colab. Replace the file-upload cell with `pd.read_csv('student-por.csv')` when running locally.

---

## Repository Structure

```
├── Regression_Project_HDS_2024__Group_10_UNP.ipynb
├── student-por.csv
├── presentation.pdf
└── README.md
```

---

*Submitted as part of HDS 2024 coursework at Bhavans Vivekananda College. For academic use only.*
