# Used Car Price Prediction using Linear and Lasso Regression

This project predicts the selling price of used cars based on various features using machine learning models. The dataset used for this project is sourced from [Kaggle](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho). The project demonstrates the use of both **Linear Regression** and **Lasso Regression** for price prediction.

## Table of Contents
- [Dataset](#dataset)
- [Project Overview](#project-overview)
- [Setup Instructions](#setup-instructions)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset contains information about used cars, such as car name, year of manufacture, fuel type, and seller type, which are used as input features to predict the selling price. 

**Columns in the dataset**:
- **Car_Name**: The name of the car.
- **Year**: The year of manufacture.
- **Selling_Price**: The price for which the car was sold (Target).
- **KM_Driven**: The total kilometers driven.
- **Fuel_Type**: The type of fuel used (Petrol, Diesel, CNG).
- **Seller_Type**: Whether the seller is a dealer or an individual.
- **Transmission**: Manual or automatic transmission.
- **Owner**: Number of previous owners.

For more details, you can check the dataset on [Kaggle](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho).

## Project Overview

This project consists of the following steps:
1. Data Preprocessing: 
   - Handle missing values.
   - Encode categorical variables (Fuel_Type, Seller_Type, Transmission).
2. Exploratory Data Analysis (EDA):
   - Visualize data distribution.
   - Analyze the relationships between variables and the target feature (Selling_Price).
3. Model Training:
   - Use **Linear Regression** and **Lasso Regression** models to predict car prices.
   - Evaluate the models based on R-squared error and visualize the results.
4. Model Evaluation:
   - Compare the accuracy and performance of both models on test data.
   
## Setup Instructions

Follow these steps to set up the project and run the code:

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/car-price-prediction.git
cd car-price-prediction
```

### 2. Create a Virtual Environment (Optional)

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

Install the required Python libraries using `pip` from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

To generate `requirements.txt` based on your environment, run:

```bash
pip freeze > requirements.txt
```

### 4. Run the Project

Execute the script to run the model training and testing:

```bash
python car_price_prediction.py
```

## Project Workflow

1. **Loading the Dataset**: The data is loaded into a Pandas DataFrame, and basic exploratory steps are performed to inspect the data.
2. **Data Preprocessing**:
   - Missing values are checked, and categorical variables are encoded (e.g., Fuel_Type, Seller_Type, Transmission).
   - The target variable is `Selling_Price`, and the feature set is the remaining columns.
3. **Train-Test Split**: The data is split into training and test sets (90% train, 10% test).
4. **Model Training**:
   - **Linear Regression**: A linear regression model is trained to predict selling prices.
   - **Lasso Regression**: Lasso regression is also used to predict prices as an alternative to linear regression.
5. **Model Evaluation**:
   - The models are evaluated using R-squared error.
   - Predictions are compared to actual values using scatter plots for visualization.
6. **Visualization**:
   - Actual prices vs predicted prices are plotted for both training and test sets.

## Results

Both **Linear Regression** and **Lasso Regression** were used for the prediction task:

- **Linear Regression**:
  - R-squared error on training data: **X.XX**
  - R-squared error on test data: **X.XX**
  
- **Lasso Regression**:
  - R-squared error on training data: **X.XX**
  - R-squared error on test data: **X.XX**

Example of actual prices vs predicted prices scatter plot:
![Actual vs Predicted Prices](example_plot.png)

## Contributing

Contributions are welcome! If you have suggestions for improving the project, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```
