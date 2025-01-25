# Project-Machine-Learning-Medical-Insurance-Cost-Prediction

## Project Overview
The goal of this project was to develop a predictive system that estimates insurance charges based on demographic, lifestyle, and medical factors. 

The dataset used contains features such as age, sex, BMI, number of children, smoking habits, and region. By leveraging machine learning techniques, specifically Multiple Linear Regression (MLR) and Random Forest Regression (RFR), we aimed to identify the key predictors of insurance costs and create robust models for accurate cost estimation.

## Motivation
Predicting insurance costs is crucial for both insurance companies and policyholders. 

Insurance providers can use such models to assess risk and set premiums, while policyholders can gain insights into how their personal and lifestyle factors influence costs. 

This project demonstrates the power of machine learning in solving real-world business problems.

## Steps Undertaken
### 1. Data Preprocessing
Dataset Used: A publicly available dataset containing information about insurance costs and corresponding features.
#### Preprocessing Steps:

Handled missing data (if any).

Applied label encoding to categorical variables (e.g., sex, smoker, and region) to convert them into numerical form for model compatibility.

Performed exploratory data analysis (EDA) to understand feature distributions and relationships with the target variable (charges).

Checked for multicollinearity among features to ensure reliable regression model performance.

### 2. Exploratory Data Analysis (EDA)
EDA helped us uncover key trends in the dataset:

Smoking had the most significant impact on insurance charges.

BMI and age were positively correlated with insurance costs.

Regional differences showed minimal effect on insurance charges.

### 3. Model Building
We implemented and compared two machine learning models:

Multiple Linear Regression (MLR): A simple linear approach that assumes a linear relationship between predictors and the target variable.

Random Forest Regression (RFR): A more sophisticated ensemble learning method capable of capturing complex, non-linear patterns in the data.

#### Steps for Each Model:
Split the data into training and test sets (80% training, 20% testing).

Trained the models using the training set.

Evaluated performance using metrics such as:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

### 4. Evaluation Results
#### Multiple Linear Regression Results:
R² Score: ~0.75

RMSE: ~6060 USD

#### Random Forest Regression Results:
R² Score: ~0.83

RMSE: ~4932 USD


### Conclusion: The Random Forest Regression model outperformed Linear Regression due to its ability to capture non-linear relationships in the data.

### 5. Prediction System
We built a prediction system for both models to estimate insurance charges based on user-provided inputs such as age, BMI, smoking habits, and region. For instance:

Sample input: (Age: 30, Sex: Male, BMI: 29.0, Children: 2, Smoker: Yes, Region: Southeast)

MLR Predicted Cost: ~27662 USD

RFR Predicted Cost: ~19235 USD

This system highlights the models’ practical applicability for real-world scenarios.

### 6. Visualization
To better understand the models’ behavior:

Plotted actual vs predicted charges for both models, highlighting the discrepancies and the effectiveness of each model.

Created residual plots and error histograms to analyze model performance further.

## Key Insights
1. Smoking was the most critical factor in determining insurance charges.
2. BMI and age had strong positive correlations with charges, indicating their substantial influence.
3. Random Forest Regression captured more nuanced patterns than Linear Regression, resulting in better predictions.


## Challenges and Lessons Learned
Balancing simplicity (MLR) and complexity (RFR) was crucial. While RFR provided better accuracy, MLR was more interpretable.

Feature encoding methods (e.g., label encoding vs. one-hot encoding) influenced model outputs, emphasizing the importance of preprocessing.

Visualizing model performance helped in identifying and diagnosing model limitations.

## Future Work
Hyperparameter Tuning: GridSearchCV or RandomizedSearchCV could further optimize the Random Forest model.

Advanced Models: Experimenting with gradient boosting models (e.g., XGBoost) could improve prediction accuracy.

Feature Engineering: Adding interaction terms or external data (e.g., medical history) might enhance model performance.

## Conclusion
### This project demonstrated the application of machine learning in predicting insurance costs. The Random Forest Regression model provided the best performance, emphasizing the importance of ensemble methods for non-linear data. By developing a prediction system and visualizing results, we showcased how such models could be applied in real-world scenarios, offering valuable insights for both insurance providers and customers.

## Closing Remarks
### This project was a valuable opportunity to explore data preprocessing, regression analysis, model evaluation, and visualization techniques. It also highlighted the importance of selecting the right machine learning approach based on the problem context and dataset. By integrating predictive models and user-friendly systems, this project lays the groundwork for further innovation in cost prediction.

