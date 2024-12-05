# Recipe-Site-Popularity-Prediction
 
## Project Overview
This project aims to classify recipes as either "High Traffic" or "Low Traffic" using machine learning. By leveraging Logistic Regression and Random Forest models, the goal is to optimize recipe selection for Tasty Bytes' homepage, driving user engagement and increasing subscriptions.

## Business Goals
- Develop a machine learning solution to improve decision-making for recipe selection.
- Predict which recipes are likely to generate high traffic, achieving at least 80% accuracy in classification.
- Minimize the likelihood of showing low-traffic recipes to maximize user engagement and subscriptions.

## Dataset
The dataset includes nutritional information, categories, servings, and traffic labels for recipes. Preprocessing steps included:
- Handling missing values with median imputation.
- Cleaning categorical data (e.g., merging redundant categories).
- Ensuring correct data types and standardizing features for modeling.

## Exploratory Analysis
Key findings from the dataset:
- **Categories:** Vegetables, Potatoes, and Pork are strong predictors of high traffic.
- **Nutrients:** Calorie and protein content showed no strong correlation with traffic levels.
- **Class Imbalance:** The dataset contains slightly more high-traffic recipes than low-traffic recipes.

## Models
Two machine learning models were developed:
1. **Logistic Regression**
2. **Random Forest**

### Key Metrics
- **Precision:** How well the model avoids predicting low-traffic recipes as high traffic.
- **Recall:** The ability to identify all high-traffic recipes.
- **F1-Score:** Balances Precision and Recall.
- **AUC-ROC:** Measures the model's ability to distinguish between high and low traffic.
- **Accuracy:** Overall correctness of predictions.

## Results
- **Logistic Regression** outperformed Random Forest, with a higher AUC-ROC (0.86) and better precision (0.85).
- The model effectively minimizes misclassifications, making it the preferred choice for deployment.

## Recommendations
- Validate the Logistic Regression model on new recipes to ensure robust performance.
- Deploy the model via API or platform integration for real-time predictions.
- Prioritize high-impact categories like Vegetables and Potatoes for recipe recommendations.
- Collect more data on underrepresented categories to improve model accuracy.
- Continuously monitor and retrain the model with updated data.

## Repository Contents
The repository contains the following files:

- `data/recipe_site_traffic_2212.csv`: The raw dataset used for this project.
- `predicting_recipe_popularity.ipynb`: The Jupyter Notebook containing the code for data preprocessing, exploratory analysis, model training, and evaluation.
- `Recipe-Popularity-Prediction-Report.pdf`: The final presentation summarizing the project, findings, and recommendations.

These files collectively provide a comprehensive view of the project, from data analysis to actionable insights.
