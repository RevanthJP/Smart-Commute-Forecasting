# **Smart Commute Forecasting**

## **Project Overview**  
This project aims to analyze and predict employees' preferred modes of transportation based on key factors such as age, salary, work experience, distance, and more. Using machine learning models, we provide insights into commuting patterns and recommend optimal transport solutions for a consulting company. This enhances employee satisfaction and optimizes transportation services.

---

## **Dataset Description**  
The dataset contains 9 key features describing employees' commuting patterns:

| **Feature**       | **Description**                                                      |
|-------------------|----------------------------------------------------------------------|
| `Age`             | Age of the employee (in years).                                       |
| `Gender`          | Gender of the employee (`Male`/`Female`).                             |
| `Engineer`        | Engineer status: `1` for Engineer, `0` for Non-Engineer.              |
| `MBA`             | MBA qualification: `1` for MBA, `0` for Non-MBA.                     |
| `Work Exp`        | Total work experience (in years).                                     |
| `Salary`          | Annual salary (in lakhs per annum).                                   |
| `Distance`        | Distance from home to office (in kilometers).                         |
| `License`         | Driving license status: `1` for Yes, `0` for No.                      |
| `Transport`       | Mode of transport preferred (target variable).                        |

---

## **Exploratory Data Analysis (EDA)**  

### **Key Insights from Descriptive Statistics:**  
- **Average Age:** 28 years (Range: 18 to 43 years).  
- **Average Distance Travelled:** 11 km (Range: 1 km to 30 km).  
- **Salary Range:** ₹7L to ₹18L per annum, with an average salary of ₹12.5L.  
- **Work Experience:**  
  - 65% of employees have 0-5 years of experience.  
  - 25% have 5-10 years of experience.  
  - 10% have more than 10 years of experience.  
- **License Holders:** 60% of employees have a driving license.  
- **Transport Mode Preferences:**  
  - 50% prefer public transport.  
  - 30% prefer private vehicles.  
  - 20% prefer company-provided shuttles.

---

## **Data Preprocessing & Model Building**  
1. **Data Splitting:**  
   - **Training Set:** 70%  
   - **Test Set:** 30%  

2. **Feature Scaling:**  
   - Applied MinMaxScaler to ensure uniformity across numerical features.

3. **Models Implemented:**  
   - **Logistic Regression**  
   - **Linear Discriminant Analysis (LDA)**  
   - **Decision Tree Classifier (CART)**  
   - **Naïve Bayes**  
   - **K-Nearest Neighbors (KNN)**  
   - **Random Forest**  
   - **Gradient Boosting**

---

## **Model Performance Comparison**  

| **Model**                  | **Training Accuracy** | **Test Accuracy** | **AUC-ROC (Train/Test)** |
|----------------------------|----------------------|-------------------|--------------------------|
| Logistic Regression         | 89%                  | 88%               | 0.87 / 0.85              |
| Linear Discriminant Analysis | 85%                  | 80%               | 0.81 / 0.78              |
| Decision Tree Classifier     | 82%                  | 78%               | 0.76 / 0.74              |
| Naïve Bayes                 | 75%                  | 70%               | 0.68 / 0.66              |
| KNN                         | 77%                  | 72%               | 0.70 / 0.68              |
| Random Forest               | 91%                  | 89%               | 0.89 / 0.87              |
| Gradient Boosting           | 86%                  | 83%               | 0.83 / 0.81              |

---

## **Business Insights & Recommendations**  
1. **Transport Patterns:**  
   - Employees without driving licenses are **30% more likely** to prefer public transport.  
   - Male employees with higher work experience and salaries above ₹15L are **40% more likely** to prefer private vehicles.

2. **Data Gaps Identified:**  
   - Lack of data on employee satisfaction with their current transport mode.  
   - Missing information on reasons for not holding licenses.  
   - No data on employees' willingness to switch transport modes.

3. **Recommendations:**  
   - Conduct employee surveys to gather qualitative insights.  
   - Introduce company-provided transport services for long-distance commuters.  
   - Offer transport incentives, such as fuel allowances, to encourage private vehicle use where feasible.

---

## **Conclusion**  
The **Random Forest** and **Logistic Regression** models consistently delivered the best results in terms of accuracy, AUC-ROC scores, and overall reliability. Implementing these models can help the organization make data-driven decisions to improve employee commuting options, reducing transit-related stress and boosting overall satisfaction.

---


