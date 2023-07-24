# PROJECT-BIKE-SHARING

README for Bike Demand Prediction Project

### Bike Demand Prediction Project

This project aims to model the demand for shared bikes for a US bike-sharing provider, BoomBikes. The company has experienced revenue decline due to the ongoing Covid-19 pandemic and wants to understand the factors affecting bike demand in the American market. The goal is to build a predictive model that can help the management understand how the demand varies with different features and adjust their business strategy accordingly to meet customer expectations and improve revenue.

### Dataset

The dataset contains daily bike demand data across the American market based on various meteorological surveys and people's styles. It includes several independent variables like 'season', 'weathersit', 'temperature', 'humidity', etc., and the target variable 'cnt' representing the total number of bike rentals.

### Data Preparation

- Convert numeric values of 'weathersit' and 'season' into categorical string values based on the data dictionary.
- Consider the 'yr' column with values 0 and 1 representing the years 2018 and 2019. Since bike-sharing systems are gaining popularity, retain the 'yr' column as it may be a good predictor for bike demand.

### Model Building

- The target variable is 'cnt', which represents the total number of bike rentals.
- Build a predictive model using appropriate regression algorithms (e.g., Linear Regression, Decision Tree Regression, Random Forest Regression).
- Split the data into training and testing sets.

### Model Evaluation

- Evaluate the performance of the model on the test set using the R-squared (R²) score.
- Calculate the R-squared score using the provided code:
```python
from sklearn.metrics import r2_score
r2_score(y_test, y_pred)
```

### Steps to Reproduce the Results

1. Load the dataset and explore its contents.
2. Preprocess the data by converting numeric values of 'weathersit' and 'season' into categorical string values and considering the 'yr' column.
3. Visualize the data to gain insights into the relationships between different variables and the target variable 'cnt'.
4. Choose relevant features and drop any irrelevant or redundant ones.
5. Split the data into training and testing sets.
6. Build the predictive model using regression algorithms and train it on the training set.
7. Evaluate the model's performance on the test set using the R-squared score.
8. Interpret the model coefficients and analyze the significant variables affecting bike demand.
9. Provide meaningful insights and recommendations based on the model's findings.

### Conclusion

The predictive model will help BoomBikes understand the demand dynamics of the American market after the Covid-19 quarantine situation ends. It will enable them to make informed business decisions, meet customer needs, and accelerate their revenue once the economy recovers.

Note: The provided code for calculating the R-squared score is crucial for evaluation and should not be omitted.
