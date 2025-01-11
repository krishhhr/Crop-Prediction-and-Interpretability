# Crop Prediction Based on Soil Analysis and Weather Prediction

This project explores the use of **machine learning (ML)** techniques to recommend optimal crops based on environmental and soil parameters. By leveraging advanced ML models and **Explainable AI (XAI)** methods, we aim to enhance agricultural productivity and sustainability.

![Header Image](https://via.placeholder.com/1200x400.png?text=Crop+Prediction+Project) <!-- Replace with actual image URL -->

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

![Correlation Heatmap](https://via.placeholder.com/600x400.png?text=Heatmap+Placeholder) <!-- Replace with actual heatmap -->

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

![Scatter Plot](https://via.placeholder.com/600x400.png?text=Scatter+Plot+Placeholder) <!-- Replace with actual scatter plot -->

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
  
![Model Accuracy Comparison](https://via.placeholder.com/600x400.png?text=Model+Comparison+Placeholder) <!-- Replace with actual accuracy chart -->

### Detailed SHAP Analysis
- **Rice:** High humidity and rainfall were significant factors.
- **Cotton:** Warm temperatures and potassium improved yields.
- **Papaya:** Thrives in humid, warm climates.

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
