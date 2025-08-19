# 🎓 Student Score Prediction

This project focuses on predicting **student exam performance** based on academic, socio-economic, and personal factors using **Machine Learning**.  
The goal is to analyze key factors, perform feature selection, and build regression models to evaluate prediction accuracy.

---

## 📊 Dataset
- **Records:** 6,607 students  
- **Features:** Academic performance, study habits, parental involvement, family income, access to resources, motivation level, and more.  
- **Target:** `Exam_Score`

---

## 🛠 Project Workflow
1. **Data Cleaning & Preprocessing**
   - Handled missing values using mode imputation
   - Outlier detection with IQR method
   - One-hot encoding for categorical variables
   - Normalization using MinMaxScaler

2. **Exploratory Data Analysis (EDA)**
   - Boxplots & histograms for distribution analysis  
   - Correlation heatmap for numeric features  
   - ANOVA & Eta-Squared for categorical importance  

3. **Feature Selection**
   - Manual selection based on statistics & visualization  
   - Automatic selection using `SelectKBest (f_regression)`  

4. **Modeling**
   - **Linear Regression** on:
     - Manually selected features  
     - SelectKBest features  
     - Raw dataset  
   - **Polynomial Regression** (degree=2) on raw dataset  

5. **Evaluation**
   - Metrics: R² Score, Mean Squared Error (MSE)  
   - Visualizations: True vs Predicted plots, residuals distribution, model comparison bar chart  

---

## 📈 Results
- **Linear Regression (Raw dataset)** performed best:  
  - Train R² ≈ **0.717**  
  - Test R² ≈ **0.770**  
  - MSE ≈ **3.26**  

- Polynomial Regression slightly underperformed compared to Linear Regression.  

---

## 🖥 Tech Stack
- Python  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn  
- Google Colab  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/ahmedmostafa2112/student-score-prediction.git
   cd student-score-prediction
