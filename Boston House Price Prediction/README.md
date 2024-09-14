**Boston House Price Prediction**

**Step 1: Load and Preprocess the Data**

# Boston House Price Prediction

This project demonstrates the prediction of house prices using a dataset of Boston housing data, which includes various factors such as crime rates, number of rooms, and more. It utilizes several regression models, focusing on data preprocessing, model selection, and evaluation to predict the house prices accurately.

## Dataset

The dataset contains attributes such as:
- **CRIM:** Per capita crime rate by town
- **RM:** Average number of rooms per dwelling
- **AGE:** Proportion of owner-occupied units built prior to 1940
- **TAX:** Full-value property-tax rate per $10,000
- **MEDV:** Median value of owner-occupied homes (Target)

## Models Used
1. **Linear Regression**
2. **Gradient Boosting Regressor** (Primary model)
3. **Decision Tree (optional)**

## Key Steps
### 1. Data Preprocessing
- **Missing Value Imputation:** Handled using the mean imputation strategy.
- **Outlier Detection:** Boxplots used to visualize and handle potential outliers.
- **Feature Scaling:** Standardized features using `StandardScaler` to ensure all features have equal importance.

### 2. Model Selection
- Multiple models were tested, but the final model is a tuned **Gradient Boosting Regressor** for the best performance.

### 3. Training and Testing
- The data is split into **80% training** and **20% testing** sets.
- The model was trained using the training data and evaluated using the test data.

### 4. Evaluation
- The performance is measured using **Mean Squared Error (MSE)** and **R-squared (R²)** score.
  


