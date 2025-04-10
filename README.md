# Banglore_House_Price_Prediction
A machine learning model that predicts house price using DecisionTreeRegressor



1. Objective:

-To predict house prices in Bangalore based on various features like area type, location, size, total square footage, number of bathrooms, balconies, and more.

2. Dataset:

-The dataset contains 13,320 records and 9 columns including area_type, availability, location, size, total_sqft, bath, balcony, and price.

-Loaded from a CSV file using pandas.

3. Data Cleaning:

-Dropped the society column due to high number of missing values.

-Handled null values:

   -Replaced missing values in location and size with their mode.

   -Filled missing numerical values (bath, balcony, total_sqft) using mean imputation with SimpleImputer.

4. Feature Engineering:

-Converted total_sqft values like "1000-1200" to their average.

-Encoded categorical variables using:

-Label Encoding for area_type, availability, location, and size.

-Converted availability into three categories: Ready to Move, Immediate Possession, and Delayed.

5. Feature Scaling:

-Applied StandardScaler to scale features for better model performance.

6. Splitting Data:

-Split dataset into training and test sets using train_test_split with an 80-20 ratio.

7.Model Building:

-Used DecisionTreeRegressor from scikit-learn to train the model on the processed dataset.
