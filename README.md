# BanglorePricePrediction

1. **Data Preprocessing**:
   - The dataset initially had 13,320 entries and 9 columns.
   - After dropping unnecessary features (area_type, society, balcony, availability), the dataset was reduced to 13,320 rows and 5 columns (location, size, total_sqft, bath, price).
   - Null values were handled, resulting in a final dataset (df2) with 13,246 rows and no missing values.

2. **Feature Engineering**:
   - Created new features:
     - bhk (Bedrooms, Hall, Kitchen) derived from the size column.
     - price_per_sqft calculated as price / total_sqft.

3. **Dimensionality Reduction**:
   - Tagged locations with fewer than 10 data points as 'Other' to reduce the number of distinct categories before one-hot encoding.

4. **Outlier Detection and Removal**:
   - Outliers were identified and removed using various methods (Business Logic, Standard Deviation and Mean, Bathrooms Feature) to enhance model robustness.

5. **Model Building and Evaluation**:
   - Trained and evaluated multiple regression models:
     - **Linear Regression**: Tuned for fit_intercept.
     - **Lasso Regression**: Tuned for alpha (regularization strength) and selection method (random vs cyclic).
     - **Decision Tree Regression**: Tuned for criterion (mse vs friedman_mse) and splitter (best vs random).

6. **Model Selection**:
   - Used GridSearchCV for hyperparameter tuning and cross-validation (5-fold) to find the best performing model for predicting home prices.
   - The results of GridSearchCV provided the best scores and parameters for each model (linear_regression, lasso, decision_tree).

7. **Prediction Function**:
   - Created a function (predict_price) to predict home prices based on user-provided inputs of location, square footage (sqft), number of bathrooms (bath), and bedrooms (bhk).

Overall, the notebook demonstrated a structured approach to data preprocessing, feature engineering, outlier management, model selection, and evaluation, culminating in a predictive model for home prices in Bangalore. The process aimed to optimize model performance and provide accurate predictions for real-world applications in the real estate domain.


# Name :Chandekar Dhruvin

**Email : dhruvinchandekar@gmail.com**
**Linkedin : www.linkedin.com/in/chandekar-dhruvin**

**Portfolio :- https://www.datascienceportfol.io/Dhruvin**

# Projects

**1. Car Price Prediction :- https://github.com/ChandekarDhruvin/Cars24-Data-Analysis**

**2. Amazon Sales Analysis :- https://github.com/ChandekarDhruvin/Amazon_Sales_Analysis**

**3. Retail Store Data :- https://github.com/ChandekarDhruvin/OIBSIP_Task01-RetailStoreData**

**4. House Price Prediction :- https://github.com/ChandekarDhruvin/OIBSIP_Task03-House_Price_Prediction**

**5. ECommerce Purchase :- https://github.com/ChandekarDhruvin/ECommerce-Purchase**

**6. Wine Quality Prediction :- https://github.com/ChandekarDhruvin/OIBSIP_Task04-WineQuality_Prediction**

**7. New York AirBNB Data Analysis :- https://github.com/ChandekarDhruvin/OIBSIP_Task02-NewYork_AirBnb_Data_Analysis**

**8. AdultData Analysis :- https://github.com/ChandekarDhruvin/AdultDataSet_analysis**

**9. Diwali Sales Data Analysis :- https://github.com/ChandekarDhruvin/Diwali-Sales-Data-Analysis**



