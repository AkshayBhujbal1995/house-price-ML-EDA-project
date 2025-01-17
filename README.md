# House Price Analysis and Prediction

This project analyzes housing data from King County, USA, obtained from Kaggle, and builds predictive models for house prices. The aim is to identify key factors influencing house prices and create models to predict prices accurately.


## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset Description](#dataset-description)  
3. [Technologies Used](#technologies-used)  
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis)  
5. [Modeling](#modeling)  
6. [How to Use the Code](#how-to-use-the-code)  
7. [Results](#results)  
8. [Conclusion](#conclusion)  
9. [Future Work](#future-work)  


## Project Overview  

This project explores the relationships between various housing features and their impact on prices. Using statistical and machine learning techniques, the project aims to extract insights and create accurate predictive models.


## Dataset Description  

The dataset is sourced from Kaggle: [House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction). It includes 21 columns describing housing characteristics:

- **Features**:  
  - `date`: Date of sale.  
  - `bedrooms`: Number of bedrooms.  
  - `bathrooms`: Number of bathrooms.  
  - `sqft_living`: Square footage of living space.  
  - `sqft_lot`: Square footage of the lot.  
  - `floors`: Number of floors.  
  - `waterfront`: Binary indicator for waterfront properties.  
  - `view`: Rating of property views.  
  - `condition`: Condition of the house.  
  - `grade`: Overall grade of the house based on King County grading system.  
  - `sqft_above`: Square footage of the house apart from the basement.  
  - `sqft_basement`: Square footage of the basement.  
  - `yr_built`: Year the house was built.  
  - `yr_renovated`: Year the house was renovated (if applicable).  
  - `zipcode`: ZIP code of the house location.  
  - `lat`: Latitude of the house location.  
  - `long`: Longitude of the house location.  
  - `sqft_living15`: Average square footage of living space for the 15 closest homes.  
  - `sqft_lot15`: Average square footage of lot space for the 15 closest homes.  

- **Target**:  
  - `price`: Price of the house.  


## Technologies Used  

- **Programming Language**: Python  
- **Libraries**:  
  - `pandas` for data manipulation  
  - `numpy` for numerical computations  
  - `matplotlib` and `seaborn` for data visualization  
  - `scikit-learn` for machine learning  
  - `datetime` for date handling  


## Exploratory Data Analysis  

Key steps in EDA included:  
- **Data Cleaning**: Checked for missing or inconsistent values.  
- **Data Transformation**: Converted the `date` column to `datetime` format.  
- **Correlation Analysis**:  
  - Features like `sqft_living` and `grade` showed strong positive correlations with `price`.  
  - Features like `zipcode` and `long` had weak correlations.  


## Modeling  

- **Regression Models Used**:  
  - Simple Linear Regression  
  - Multiple Linear Regression  
  - Ridge Regression  
  - Polynomial Regression  

- **Evaluation Metrics**:  
  - R² Score  
  - Mean Squared Error (MSE)  

- **Performance Highlights**:  
  - **Best R² Score**:  
    - Multiple Linear Regression: 0.711 (Test Data)  
    - Ridge Regression with Polynomial Features: 0.700  


## How to Use the Code  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/house-price-analysis.git  
   ```  
2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  
3. Run the analysis:  
   ```bash  
   jupyter notebook analysis.ipynb  
   ```  


## Results  

The project demonstrates:  
- **Significant predictors** of house prices: `sqft_living`, `grade`, `bathrooms`.  
- **Negligible predictors**: `zipcode`, `long`.  
- Regression models provide reliable predictions, with an R² score of up to 0.711 for test data.  


## Conclusion  

The analysis confirms that factors like living area, house grade, and number of bathrooms significantly influence house prices. Machine learning models, especially Multiple Linear Regression, effectively predict house prices.  


## Future Work  

- Explore advanced machine learning models like Random Forest or Gradient Boosting.  
- Perform feature engineering to create new predictors.  
- Use additional datasets for a broader analysis.  
