# Healthcare Analysis and Sales Enchanement
This project aims to analyze healthcare trends and enhance hospital revenue based on patient demographics, medical conditions, and other features. Using machine learning, we develop a predictive model for hospital billing and visualize key insights related to healthcare costs, patient conditions, and hospital stays. The repository contains the Python code for the machine learning model and a Tableau dashboard showcasing key healthcare metrics.

---

## 1. Project Overview

Accurate billing prediction is critical for hospitals to optimize resources and manage costs effectively. This project leverages patient data to build a predictive model for hospital billing and explores trends in patient demographics, medical conditions, and healthcare costs.

### Key Objectives:
- Analyze patient data to uncover key factors influencing healthcare costs.
- Build a machine learning model to predict hospital billing amounts based on various patient features.
- Visualize healthcare trends and costs using Tableau for better decision-making.

---

## 2. Features and Approach

### 2.1 Data Preparation
The dataset includes various features such as:

- **Patient Demographics** (Age, Gender, Blood Type)
- **Medical Conditions** (Diabetes, Cancer, Obesity, etc.)
- **Admission and Discharge Details** (Date of Admission, Discharge Date, Room Type)
- **Billing Information** (Billing Amount, Insurance Provider)

### 2.2 Feature Engineering
We applied feature engineering to improve the model’s predictive performance:

- **Length of Stay**: Calculated by the difference between Discharge Date and Date of Admission to understand how long patients stay in the hospital.
- **AgeAbove50_Cancer_PrivateRoom**: A binary feature to capture the interaction between patients over 50 years old with cancer staying in Special Private rooms, which may drive higher billing.
- **Categorical Variables**: Medical conditions, room types, and insurance providers were transformed using one-hot encoding for better model interpretability.

### 2.3 Model Building
A decision tree-based regression model was developed to predict the hospital billing amount. 

**Key Model Results**:
After feature engineering, the model’s accuracy improved, achieving lower Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) metrics, providing a reliable prediction of hospital billing amounts.

---

## 3. Files in This Repository

### 3.1 Python ML Code (Healthcare_Billing_Prediction.ipynb)
This Python script contains the complete code for:

- Data preprocessing and feature engineering.
- Model building, training, and evaluation.
- Model performance metrics such as MAE and RMSE.
  
You can run the code to reproduce the results or experiment with different models and parameters.

### 3.2 Tableau Dashboard (Healthcare_Dashboard.png)
This is a screenshot of the Tableau dashboard visualizing key insights, including:

- Cost distribution across medical conditions.
- Billing trends based on room types and medical conditions.
- Patient demographics and their impact on healthcare billing.
  
The dashboard provides a comprehensive view of healthcare costs and patient data.

### 3.3 Dataset (Healthcare_Data.csv)
This dataset contains the patient data used for the project. You can upload this dataset to your environment (e.g., Google Colab) and adjust the file path in the Python code to run the analysis on your setup.

The Tableau dashboard visualizes healthcare data, providing clear insights into patient behavior, medical conditions, and costs.

---

## 4. Getting Started

### Prerequisites:
- **Python 3.x**
- Required libraries: pandas, numpy, sklearn, matplotlib, etc.
- **Tableau** for data visualization

---

## 5. Results and Conclusion

### Model Performance:
- The model achieved **Mean Absolute Error (MAE)** of **18,994.80** and **Root Mean Squared Error (RMSE)** of **22,247.20** after feature engineering, providing accurate predictions of hospital billing.

### Insights:
- The model identified that **age**, **medical condition (cancer)**, and **room type (Special Private)** were key drivers of hospital billing.
- **Insurance providers** such as Medicare and UnitedHealthcare were associated with reduced billing amounts.

### Visualizations:
- The **Tableau dashboard** offers a detailed view of healthcare trends, such as cost distribution by medical condition, room type, and patient demographics, allowing hospital administrators to make data-driven decisions.

---

## 6. Future Work

### Model Improvements:
- Explore other machine learning algorithms like Random Forest or Gradient Boosting to further improve accuracy and billing prediction.

### New Features:
- Introduce additional features, such as patient treatment history or medication costs, to enhance prediction quality.

### Deployment:
- Implement model deployment using Flask or Django to integrate billing predictions into hospital management systems for real-time decision-making.

---

This README file provides an overview of the **Healthcare Analysis and Billing Prediction** project, outlining the objectives, approach, and results, along with next steps for further improvement and deployment.


