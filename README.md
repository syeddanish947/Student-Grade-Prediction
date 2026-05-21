# 📚 Student Performance Prediction using Machine Learning

This project predicts student performance in secondary education using Machine Learning techniques and socio-demographic data. The aim is to identify factors affecting academic performance and build predictive models to help improve educational outcomes.

## 🎯 Objective
Develop and compare multiple machine learning models to identify the best approach for predicting student performance and enabling targeted educational interventions.

## 📊 Dataset
- Source: UCI Machine Learning Repository
- Dataset: Student Performance Dataset
- Records: 649
- Features: 33 variables
- Includes academic, family, and socio-demographic attributes

## 🛠 Data Preprocessing
- Checked and handled missing values
- Removed unnecessary variables (G1, G2)
- Applied dummy encoding to categorical features
- Performed multicollinearity analysis using VIF

## 📈 Exploratory Data Analysis (EDA)
Performed:
- Correlation Heatmaps
- Histograms
- Count Plots
- Pie Charts
- Box Plots
- Scatter Plots

## 🤖 Machine Learning Models Used
- Linear Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- XGBoost
- AdaBoost
- Artificial Neural Network (ANN)

## 📏 Evaluation Metrics
Models were evaluated using:
- R² Score
- MAE (Mean Absolute Error)
- RMSE

## 🏆 Best Model
Adaptive Boosting (AdaBoost) achieved the best performance:

- MAE: 1.767
- Train-Test Split: 80:20

## 🔍 Key Insights
- Study time and parental education significantly affect performance.
- Social and lifestyle factors also impact student outcomes.
- Supportive home environments positively influence academic success.

## 🚀 Future Scope
- Integrate real-time student data
- Add external educational factors
- Personalized learning recommendations
- Expand to global datasets


---
⭐ If you found this project useful, consider giving it a star.
