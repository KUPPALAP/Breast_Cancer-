# Breast Cancer Classification Using Machine Learning

## Team Members
- **Karunakar** – Implemented Random Forest Classifier  
- **Varshitha** – Implemented Gradient Boosting Classifier  
- **Saketha** – Implemented Support Vector Machine (SVM)  

## Project Overview
This project applies machine learning models to classify breast cancer as **malignant (cancerous) or benign (non-cancerous)** using the **Breast Cancer Wisconsin Dataset**. The focus is on **Random Forest Classifier**, which is known for its robustness and high accuracy. The dataset was preprocessed, models were trained with hyperparameter tuning, and the final model was evaluated based on key performance metrics.

## Dataset Description
The dataset, provided by Scikit-learn, consists of **569 samples** with **30 numerical features** extracted from digitized images of breast masses. Features include:
- **Mean values** (e.g., radius, texture, perimeter, area, smoothness)
- **Worst values** (largest tumor measurements)
- **Error values** (standard errors of features)

### Target Variable:
- **0 → Malignant (cancerous)**
- **1 → Benign (non-cancerous)**

## Methodology
1. **Data Collection** – Using the Breast Cancer Wisconsin dataset.  
2. **Data Preprocessing** – Cleaning, normalizing, and splitting the data.  
3. **Model Selection** – Comparing different machine learning classifiers.  
4. **Hyperparameter Tuning** – Optimizing model performance using **GridSearchCV**.  
5. **Model Evaluation** – Measuring **accuracy, precision, recall, and F1-score**.  
6. **Conclusion** – Assessing model performance and discussing improvements.

## Data Preprocessing
- **Checked for missing values** – No missing values were found.  
- **Feature Scaling** – Standardized all features using **StandardScaler**.  
- **Train-Test Split** – Dataset split into **80% training and 20% testing**.  

## Model Selection and Hyperparameter Tuning

### **Random Forest Classifier (Implemented by Karunakar)**
Random Forest is an ensemble learning method that improves accuracy by combining multiple decision trees.

#### **Hyperparameter Tuning (GridSearchCV)**
The model was optimized using **GridSearchCV**, testing the following hyperparameters:
- **n_estimators**: [50, 100, 200] (number of trees)
- **max_depth**: [None, 10, 20] (tree depth)
- **min_samples_split**: [2, 5, 10] (minimum samples required to split a node)

