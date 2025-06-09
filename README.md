# Property_Price_Prediction

# Machine_Learning_Project-Property-Price-Prediction
Property Price Prediction using Simple Linear Regression

Overview : The Property Price Prediction project utilizes Simple Linear Regression, a fundamental machine learning algorithm, to predict real estate prices based on various factors such as location, size, number of rooms, and other features. This model helps in estimating the price of properties efficiently and accurately based on historical data.

Features : Data Preprocessing: Cleaning and transforming raw real estate data for better accuracy. Feature Engineering: Selecting relevant features that influence property prices. Model Training: Implementing Multiple Linear Regression to train the model. Model Evaluation: Assessing model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²). Prediction Interface: Providing a simple interface to input property details and get price predictions.

Technologies Used : Python (for data processing and model development) Libraries: pandas (Data Manipulation) numpy (Numerical Computation) matplotlib & seaborn (Data Visualization) sklearn (Machine Learning Model) Jupyter Notebook

Model Training & Evaluation: Data Preprocessing Handling missing values and outliers. Encoding categorical variables. Feature scaling. Model Implementation Splitting dataset into training and testing sets. Applying Multiple Linear Regression to find relationships between features and property prices.

Evaluation Metrics: MSE (Mean Squared Error): Measures squared differences to penalize large errors. R² Score: Indicates how well the model explains the variability in the dataset.

# Initial Correlation Matrix

![Screenshot 2025-06-09 214904](https://github.com/user-attachments/assets/6ee819a9-a298-4564-b2d0-2d8684ef4008)

# Data Preprocessing
Cleaning and transforming raw real estate data for better accuracy. Feature Engineering: Selecting relevant features that influence property prices. Model Training: Implementing Multiple Linear Regression to train the model. Model Evaluation: Assessing model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²). Prediction Interface: Providing a simple interface to input property details and get price predictions.

![image](https://github.com/user-attachments/assets/9498eb9f-7951-462e-bfee-73c021c67195)
![image](https://github.com/user-attachments/assets/73e1f948-f622-4d33-ac6f-e99176774a19)

# Exploratory Data Analysis
# Scatter Ploting
![image](https://github.com/user-attachments/assets/8fae35dd-2888-4fa6-a957-f86bd5b6ef71)

# Box Plot for analyse outliers
![image](https://github.com/user-attachments/assets/1375596b-e038-45ac-a763-2eafa8efe4c3)

# Joint Plot
![image](https://github.com/user-attachments/assets/02ae945f-6ec7-4df3-bc15-3280e8c79148)
# after analyse 
![image](https://github.com/user-attachments/assets/ac2fb9ca-ab80-416e-a8f0-6d7c860ddc3a)

# Model Building
Model Training & Evaluation: Data Preprocessing Handling missing values and outliers. Encoding categorical variables. Feature scaling. Model Implementation Splitting dataset into training and testing sets. Applying Multiple Linear Regression to find relationships between features and property prices.

Evaluation Metrics: MSE (Mean Squared Error): Measures squared differences to penalize large errors. R² Score: Indicates how well the model explains the variability in the dataset.

![image](https://github.com/user-attachments/assets/f914bc3a-e0cc-405e-b4a3-cb6bde6d4a90)


# Data Story Telling - Interactive Dashboard & Key Insights
Note: - click View Raw to download the file dashboard property price prediction(.pbix file)
![Screenshot 2025-06-10 004550](https://github.com/user-attachments/assets/bec1d62f-3150-4526-8b09-33d21b2faec8)

![Screenshot 2025-06-10 004622](https://github.com/user-attachments/assets/2b5187af-6a87-4b73-bea4-0eee1e9e67d8)

![Screenshot 2025-06-10 004646](https://github.com/user-attachments/assets/9b2e451b-ee2f-4499-aac1-2e7bf4e5e87e)

![Screenshot 2025-06-10 004721](https://github.com/user-attachments/assets/9b32f7d2-e8be-4f21-aa8a-c1627eba0b0d)

## 📊 Dashboard Features

### 1. 📍 Map Visual
- **Visual Type**: Map
- **Latitude**: `latitude`
- **Longitude**: `longitude`
- **Size**: `median_house_value`
- **Tooltips**: `median_income`, `ocean_proximity`

### 2. 🧭 Average House Value by Ocean Proximity
- **Visual Type**: Bar Chart
- **Axis**: `ocean_proximity`
- **Value**: Average of `median_house_value`

### 3. 💵 Income vs House Value
- **Visual Type**: Scatter Plot
- **X-axis**: `median_income`
- **Y-axis**: `median_house_value`
- **Color/Legend**: `ocean_proximity`

### 4. 📈 House Value by Age
- **Visual Type**: Line Chart
- **Axis**: `housing_median_age`
- **Value**: Average of `median_house_value`

### 5. 🛏️ Room Distribution
- **Visual Type**: Histogram or Column Chart
- **Axis**: Binned `total_rooms`
- **Value**: Count

### 6. 🧮 KPI Cards
- **Average House Value**
- **Total Population**
- **Average Income**
- **Bedroom Ratio**

---

## 🧠 DAX Measures Used

```DAX
Average House Value = AVERAGE(housing[median_house_value])
Total Population = SUM(housing[population])
Average Income = AVERAGE(housing[median_income])
Room per Household = DIVIDE(SUM(housing[total_rooms]), SUM(housing[households]))
Bedroom Ratio = DIVIDE(SUM(housing[total_bedrooms]), SUM(housing[total_rooms]))







