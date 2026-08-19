# Model Evaluation Report
## House Price Prediction System

### 1. Objective

The objective of this project is to develop a machine learning regression system capable of predicting residential property prices based on property characteristics.

### 2. Dataset

The dataset contains 500 synthetic residential property records.

Input features:

- Location
- Area in square feet
- Number of bedrooms
- Number of bathrooms
- Property age
- Parking spaces
- Floor number

Target:

- Property price in Indian Rupees (`price_inr`)

### 3. Data Cleaning and Preprocessing

The following preprocessing steps were implemented:

1. Dataset loaded using Pandas.
2. Missing values inspected.
3. Duplicate records removed.
4. Numeric variables processed using median imputation.
5. Categorical location values processed using most-frequent imputation.
6. Location converted into numerical features using One-Hot Encoding.
7. Preprocessing was combined with the model in a Scikit-learn Pipeline.

### 4. Exploratory Data Analysis

EDA was performed using:

- Dataset preview
- Statistical summary
- Missing-value analysis
- Histograms
- Actual-vs-predicted visualization

The analysis helps understand the distribution of property attributes and the relationship between the input variables and house prices.

### 5. Model Development

A **Random Forest Regressor** was selected as the primary regression algorithm.

Model configuration:

| Parameter | Value |
|---|---:|
| Number of estimators | 300 |
| Maximum depth | 18 |
| Minimum samples per leaf | 2 |
| Random state | 42 |
| Training split | 80% |
| Testing split | 20% |

Random Forest was selected because it can model non-linear relationships and interactions between property features.

### 6. Evaluation Metrics

#### Mean Absolute Error (MAE)

MAE measures the average absolute difference between actual and predicted prices.

**MAE: ₹874,587.00**

#### Root Mean Squared Error (RMSE)

RMSE gives greater weight to larger prediction errors.

**RMSE: ₹1,107,077.33**

#### R² Score

R² measures the proportion of variance in property prices explained by the model.

**R² Score: 0.9875**

### 7. Results

The Random Forest model achieved an R² score of **0.9875** on the held-out test dataset.

The evaluation indicates that the model is able to capture the relationships present in this synthetic dataset effectively.

### 8. Conclusion

The project successfully implements all required components of a house price prediction system:

- Data cleaning
- Data preprocessing
- Exploratory data analysis
- Feature engineering
- Regression model development
- Model evaluation
- Prediction interface
- Model persistence

The trained model can accept new property information and produce an estimated residential property price.

### 9. Limitations

The dataset used in this project is synthetic. Therefore, the reported performance should not be interpreted as real-world property valuation accuracy.

For production deployment, the model should be trained on a large, reliable real-estate dataset containing additional variables such as:

- Exact geographical coordinates
- Neighborhood
- Property type
- Distance to schools
- Distance to hospitals
- Public transport accessibility
- Local property market trends
- Construction quality
- Amenities

### 10. Future Improvements

Possible improvements include:

1. Use a real-world housing dataset.
2. Compare Random Forest with Gradient Boosting, XGBoost and other regression algorithms.
3. Perform hyperparameter tuning.
4. Apply cross-validation.
5. Build a Streamlit web application.
6. Add interactive charts.
7. Add model explainability using SHAP.
8. Deploy the prediction application online.

### 11. Final Assessment

**Project Status: Completed**

The developed system satisfies the major requirements of the House Price Prediction System assignment.
