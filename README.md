
 🚗Car Price Prediction Using Regression Models

This repository contains a comprehensive car price prediction project utilizing regression techniques. It aims to predict car prices with a focus on accuracy and model optimization, leveraging regularization to avoid overfitting. A great resource for those exploring regression modeling and performance tuning.

---

 📌 Project Overview

This project aims to predict **car prices (MSRP) based on features such as brand, model year, fuel efficiency, and premium features. The goal is to develop a robust regression model that accurately estimates car prices while minimizing overfitting.

Key Techniques Used:
- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature Engineering  
- Regression with Regularization  
- Model Evaluation & Comparison  



 📊 Dataset Description

The dataset contains 28,143 car records with the following key features:

| Feature            | Description |
|--------------------|-------------|
| model_year         | Manufacturing year of the vehicle |
| brand              | Name of the car manufacturer |
| model              | Specific car model |
| type               | Vehicle classification (SUV, Sedan, Coupe, etc.) |
| miles_per_gallon   | Fuel efficiency (MPG) |
| premium_version    | 1 if the car has a premium variant, else 0 |
| collection_car     | 1 if the car is considered collectible, else 0 |
| msrp               | Manufacturer’s Suggested Retail Price (Target) |



 🛠 Data Preprocessing

- Handling Missing Values  
- Outlier Detection & Treatment using IQR Winsorization 
- Encoding Categorical Features 
- Feature Scaling & Normalization



 📈 Exploratory Data Analysis (EDA)

- Identified trends in **fuel efficiency, brand pricing, and premium features**
- Visualizations: **Histograms, Boxplots, Correlation Heatmaps**
- Observations:  
  - Premium & collectible cars have significantly higher prices  
  - Certain brands dominate the high-price segment



 🔮 Regression Models & Performance

 1️⃣ Polynomial Regression  
- Captured non-linear trends  
- Training Accuracy: 70.93%  
- Testing Accuracy: Extremely poor (−5.76e12%) — heavy overfitting

 2️⃣ Regularized Regression

| Model                  | Training R² | Testing R² |
|------------------------|-------------|------------|
| Lasso Regression   | 63.41%      | 62.68%     |
| Ridge Regression    | 63.40%      | 62.68%     |
| Elastic Net        | 28.30%      | 28.86%     |

Key Insights:
- Lasso and Ridge performed best** with balanced bias-variance trade-offs  
- Elastic Net underperformed**, showing poor generalization  



 📌 Key Takeaways

- Polynomial regression led to overfitting and instability.
- Lasso & Ridge were the most stable and accurate models.
- Elastic Net was not suitable** for this dataset.
- Winsorization helped mitigate outliers and improve model performance.



