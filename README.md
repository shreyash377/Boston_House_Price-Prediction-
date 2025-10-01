#  House Price Prediction using Linear Regression

This project implements a **Linear Regression model** to predict house prices based on various features from the **Boston Housing dataset**.  
The notebook covers **EDA, preprocessing, model building, and evaluation**.

---

##  Dataset
- **Source:** [Boston Housing Dataset](https://raw.githubusercontent.com/selva86/datasets/master/BostonHousing.csv)  
- **Rows:** 506  
- **Columns:** 14  
- **Target Variable:** `MEDV` – Median value of owner-occupied homes in $1000's  

### Features:
- `CRIM` – per capita crime rate by town  
- `ZN` – proportion of residential land zoned for lots over 25,000 sq.ft.  
- `INDUS` – proportion of non-retail business acres per town  
- `CHAS` – Charles River dummy variable (1 if tract bounds river; 0 otherwise)  
- `NOX` – nitric oxides concentration (parts per 10 million)  
- `RM` – average number of rooms per dwelling  
- `AGE` – proportion of owner-occupied units built prior to 1940  
- `DIS` – weighted distances to five Boston employment centres  
- `RAD` – index of accessibility to radial highways  
- `TAX` – full-value property-tax rate per $10,000  
- `PTRATIO` – pupil-teacher ratio by town  
- `B` – 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town  
- `LSTAT` – % lower status of the population  
- `MEDV` – Target (Median value of homes)  

---

##  Steps in the Project
1. **Exploratory Data Analysis (EDA)**  
   - Check null values, duplicates, and data types  
   - Visualize distributions and correlations  

2. **Data Preprocessing**  
   - Handle missing values (drop, mean/median imputation)  
   - Remove duplicates  
   - Detect and treat outliers
   -   
**Feature Engineering**  
   - Generated **Polynomial Features** to capture non-linear relationships
      
3. **Model Building**  
   - Train a **Linear Regression** model  
   - Split data into train/test sets
   - Applied **Ridge Regression** (L2 Regularization) to prevent overfitting  

4. **Evaluation Metrics**  
   - R² Score  
   - Mean Squared Error (MSE)  
   - Root Mean Squared Error (RMSE)
     
**MSE:** 0.06101536026017097
**R2:** 0.9493050207598822
**Training score:** 0.9500817896767236
**Test score:** 0.9493050207598822
**These results show the model generalizes well without overfitting.**      

---

## 📦 Requirements
Install dependencies using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
