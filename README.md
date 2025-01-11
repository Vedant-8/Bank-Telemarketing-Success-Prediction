# Bank Telemarketing Success Prediction 📞💰

## Kaggle Competition Link 🔗 
[Predict the Success of Bank Telemarketing](https://www.kaggle.com/competitions/predict-the-success-of-bank-telemarketing)

## Problem Statement 📝
The goal of this project is to predict the success of telemarketing campaigns for a bank, specifically whether a customer will subscribe to a term deposit product. The dataset includes customer demographics, past interactions, and other factors, with the target variable indicating subscription success (`yes`/`no`).

The challenge is to predict outcomes with imbalanced data and identify relationships between features that drive success.

## Approach 🔍

### 1. **Exploratory Data Analysis (EDA)** 📊
- **Data Exploration**: Investigate missing values, feature distributions, and correlations.
- **Class Distribution**: Address class imbalance through visualizations.
- **Feature Insights**: Analyze numerical and categorical data for patterns.

### 2. **Data Preprocessing** ⚙️
- Handle missing values and encode categorical features.
- Use **SMOTE** to oversample the minority class, addressing class imbalance.
- Split the dataset into training and validation sets for evaluation.

### 3. **Model Building** 🤖
- Implement machine learning models including **Logistic Regression**, **Random Forest**, and **LightGBM**.
- **Hyperparameter Tuning**: Optimize models using RandomizedSearchCV for better performance.

### 4. **Model Evaluation** 📈
- Evaluate models with **F1-score** and **classification report**.
- Compare multiple models to select the best performing one on the validation set.

### 5. **Prediction & Submission** 📥
- Generate predictions on the test dataset using the best model.
- Create a **submission.csv** file for evaluation.

## Key Outcomes 🌟
- **SMOTE** applied to balance class distribution.
- **Hyperparameter tuning** for improved model performance.
- **LightGBM** outperforms other models in terms of F1-score and overall accuracy.

## Final Model 🏆
The **LightGBM** classifier was selected as the best-performing model, achieving a strong balance between precision and recall, especially for predicting the minority class.

## Installation & Usage 🚀

1. Clone the repository:
   ```bash
   git clone https://github.com/Vedant-8/Bank-Telemarketing-Success-Prediction.git
   ```

2. Open and run the notebook (`Bank_Telemarketing_Success_Prediction.ipynb`) in Jupyter or a similar environment.

3. Generate predictions on the test set and create a `submission.csv` for evaluation.

## Libraries Used 📚
- `pandas`: Data manipulation and analysis.
- `numpy`: Numerical computations.
- `matplotlib`, `seaborn`: Data visualization.
- `sklearn`: Machine learning models and tools.
- `imbalanced-learn`: Techniques for imbalanced datasets.
- `lightgbm`: Advanced gradient boosting.
