# Crop Prediction Based on Soil Analysis and Weather Prediction

This project explores the use of **machine learning (ML)** techniques to recommend optimal crops based on environmental and soil parameters. By leveraging advanced ML models and **Explainable AI (XAI)** methods, we aim to enhance agricultural productivity and sustainability.

---

## 📖 Table of Contents
1. [Introduction](#introduction)
2. [Dataset Overview](#dataset-overview)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Discussion and Conclusion](#discussion-and-conclusion)
6. [References](#references)

---

## 🧐 Introduction
Agriculture, the backbone of many economies, faces challenges such as:
- **Climate change**
- **Soil degradation**
- **Resource scarcity**

Using data-driven ML techniques, this project optimizes crop selection, yield prediction, and resource allocation to address these challenges.

---

## 📊 Dataset Overview
The dataset contains **2,200 entries** and includes the following features:

| Feature      | Description                   |
|--------------|-------------------------------|
| `N`          | Nitrogen content              |
| `P`          | Phosphorus content           |
| `K`          | Potassium content            |
| `Temperature`| Soil temperature (°C)       |
| `Humidity`   | Ambient humidity (%)        |
| `pH`         | Soil acidity level           |
| `Rainfall`   | Rainfall levels (mm)         |

### Key Insights:
- **Nitrogen levels** range from 0–140, with an average of 68.
- **Rainfall** shows significant variation, reflecting diverse climates.
- **pH values** span 3.5–9.5, indicating varied soil types.

![Correlation Heatmap](![image](https://github.com/user-attachments/assets/05715856-a686-4ced-bd8b-80af7d858168)
) <!-- Replace with your heatmap URL -->

---

## ⚙️ Methodology

### 1. **Data Preprocessing**
- **Missing Data:** Handled with K-Nearest Neighbors (KNN) imputation.
- **Feature Scaling:** Standardized numerical features.
- **Categorical Encoding:** Applied one-hot encoding.

### 2. **Exploratory Data Analysis**
Key visualizations include:
- **Correlation heatmap:** Identified strong positive correlation between `P` (phosphorus) and crop yield.
- **Temperature vs. Humidity scatter plot.**

![Scatter Plot](![download](https://github.com/user-attachments/assets/55a93544-db7e-412f-9662-5c41b6676538)
) <!-- Replace with your scatter plot URL -->

### 3. **Model Selection**
Three models were evaluated:
- **Random Forest:** Achieved **99.7% accuracy**.
- **Gradient Boosting:** Optimized for minimal error.
- **Naive Bayes:** Used as a baseline.

### 4. **Explainable AI (XAI)**
SHAP (SHapley Additive exPlanations) values were used to:
- Interpret predictions globally and locally.
- Visualize feature importance.

---

## 🏆 Results
- **Random Forest:** Best performing model with:
  - **Accuracy:** 99.7%
  - **Precision, Recall, F1-Score:** Above 90% for all classes.
  
![Model Accuracy Comparison](![image](https://github.com/user-attachments/assets/905a0746-c27f-4cf8-bd7f-1e9f59f1dbc8)
) <!-- Replace with your accuracy comparison chart -->

### SHAP Analysis

#### 1. **Rice**
- **Key factors:** High humidity, consistent rainfall, and balanced nitrogen levels.
- **Insights:** Rice thrives in regions with sufficient water and moderate nitrogen content.
  
![SHAP Analysis for Rice](![image](https://github.com/user-attachments/assets/f927bf49-d12c-46cb-b364-70f20e0f4ac2)
) <!-- Replace with your SHAP image for rice -->

#### 2. **Cotton**
- **Key factors:** Warm temperatures and adequate potassium.
- **Insights:** Cotton benefits from potassium for strong fiber formation.
  
![SHAP Analysis for Cotton](![image](https://github.com/user-attachments/assets/427f98ae-7e73-4212-8047-59477a1d4f31)
) <!-- Replace with your SHAP image for cotton -->

#### 3. **Papaya**
- **Key factors:** Warm temperatures above 20°C, high humidity, and consistent rainfall.
- **Insights:** Papaya thrives in humid climates with moderate rainfall.
  
![SHAP Analysis for Papaya](![image](https://github.com/user-attachments/assets/d4bb1969-468c-47e8-8a26-0e7b488f584b)
) <!-- Replace with your SHAP image for papaya -->

---

## 💡 Discussion and Conclusion
- **Insights:** SHAP values aligned with agronomic principles, validating the model's reliability.
- **Impact:** This framework demonstrates the transformative potential of ML in **precision agriculture**.
- **Future Work:**
  - Include dynamic weather data.
  - Expand the dataset to cover additional crops and regions.

---

## 🔗 References
1. Breiman, L. *Random Forests*. Machine Learning, 2001.
2. Lundberg, S. & Lee, S.-I. *A Unified Approach to Interpreting Model Predictions*. NeurIPS, 2017.
3. Kumar, R. *Impact of Climatic Factors on Crop Production*. Int. J. of Environmental Research, 2020.

---

## 🎉 Acknowledgment
Special thanks to:
- **Arti Nilesh Panchal:** Dataset curation, preprocessing, and model training.
- **Krish Kamlesh Ranawat:** Model optimization, SHAP integration, and report analysis.

---

Feel free to reach out for further information or contributions! 😊
