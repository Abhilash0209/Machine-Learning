#  Car Price Prediction

This project uses machine learning models (Linear Regression and Lasso Regression) to predict the **selling price of used cars** based on features like the year of purchase, current price, kilometers driven, fuel type, seller type, and transmission type.

##  Dataset

The dataset (`car data.csv`) contains information about used cars, with the following columns:

- `Car_Name`: Name of the car
- `Year`: Year of manufacture
- `Selling_Price`: Price the owner wants to sell the car for
- `Present_Price`: Current ex-showroom price
- `Kms_Driven`: Kilometers driven
- `Fuel_Type`: Type of fuel (Petrol, Diesel, CNG)
- `Seller_Type`: Dealer or Individual
- `Transmission`: Manual or Automatic
- `Owner`: Number of previous owners

##  Data Preprocessing

- Encoding of categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`)
- Dropped `Car_Name` as it is not relevant for modeling
- Splitting into independent variables `X` and target variable `Y` (`Selling_Price`)
- Train-test split (90% train / 10% test)

##  Models Used

### 1. Linear Regression
- **Training R² Score**: ~0.88
- **Test R² Score**: ~0.84

### 2. Lasso Regression
- **Training R² Score**: ~0.84
- **Test R² Score**: ~0.87

##  Visualizations

- Scatter plots of **Actual vs Predicted Prices** for both training and testing data
- Helps to visually assess model performance

##  Libraries Used

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

##  How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/Abhilash0209/Machine-learning-.git
    cd car-price-prediction
    ```

2. Install required packages (optional but recommended to use a virtual environment):
    ```bash
    pip install -r requirements.txt
    ```

3. Run the notebook or Python script:
    ```bash
    python car_price_prediction.py
    ```

4. Make sure the `car data.csv` file is in the same directory.

##  Notes

- Categorical variables were encoded using `replace`.
- You can further enhance the model by using other regression techniques, feature engineering, or hyperparameter tuning.


