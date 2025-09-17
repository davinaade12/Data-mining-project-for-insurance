# Data-mining-project-for-insurance
Medical insurance Cost Prediction
Medical Insurance Cost Prediction
A regression-based data mining project analyzing a medical insurance dataset to predict individual medical charges from demographic and health attributes. Includes exploratory data analysis, handling missing values, data visualization, feature engineering, model building, and evaluation. Compared multiple regression models to identify key cost drivers and the most accurate predictive approach.
# Medical Cost Prediction

## 📌 Project Overview
This project analyzes and predicts **medical insurance charges** using demographic and lifestyle attributes.  
The dataset, sourced from [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance), contains **1,338 instances** with both **numerical** and **categorical** variables, making it ideal for regression and machine learning tasks.

The study involves:
- Data exploration & statistical summaries  
- Handling missing values (KNN & mode imputation)  
- Outlier detection & treatment (IQR method)  
- Feature engineering & transformation (log-scaling, one-hot encoding)  
- Regression model comparison (OLS, Random Forest, SVM)  
- Cross-validation & model evaluation  

---

## 📊 Key Insights
- **Charges Distribution:** Strongly right-skewed with extreme outliers (a small group of patients incur very high costs).  
- **Smoker Status:** The most influential predictor; smokers have significantly higher charges.  
- **BMI:** Positively correlated with charges, reflecting obesity-related health costs.  
- **Age:** Moderate influence on charges but weaker than smoking or BMI.  
- **Region:** Minimal effect, though the Southeast shows slightly higher variability.  

---

## 🛠️ Tools & Methods
- **Language & Libraries:** Python (pandas, NumPy, scikit-learn, matplotlib, seaborn)  
- **Data Source:** [Kaggle – Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)  
- **Techniques Used:**  
  - Missing values handled using **KNN imputation** (numeric) & **mode imputation** (categorical)  
  - Outliers capped with the **1.5*IQR rule**  
  - **Log transformation** applied to charges for normalization  
  - **One-Hot Encoding** for categorical features (sex, smoker, region)  
  - **Feature scaling** with StandardScaler  

---

## 📂 Repository Contents
- `Data/` → Raw and cleaned datasets (`insurance_with_NAs.csv`, `insurance_cleaned.csv`)  
- `Notebooks/` → Jupyter notebooks for data exploration, preprocessing, and modeling  
- `Report.docx` → Detailed analysis report  
- `README.md` → Project documentation  

---

## 🤖 Models & Performance
### Models Compared
- **Multiple Linear Regression (OLS)**  
- **Random Forest Regressor** 🌟 (best-performing)  
- **Support Vector Regression (SVR)**  

### Results
- **Random Forest** achieved the best predictive performance with higher **R²** and lower **MSE**, effectively capturing non-linear patterns in medical costs.  
- **SVM** struggled with skewed data and non-linearity, leading to poor variance explanation.  
- **OLS Regression** offered interpretability but lower accuracy compared to ensemble methods.  

---

## 📑 Conclusion
- **Smoker status, BMI, and age** are the strongest predictors of medical costs.  
- Tree-based models like **Random Forest** outperform linear models for complex, skewed healthcare datasets.  
- Improving predictions could involve testing **boosting methods (XGBoost, LightGBM)** or **deep learning models**.  

---

## 👩‍💻 Author
**Davina Adegboyega**  
📧 x23393686@student.ncirl.ie  

