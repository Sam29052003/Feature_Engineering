

##  Objective
To convert cleaned retail data into a **high-quality engineered dataset** suitable for:
- Machine Learning models
- Time-series forecasting
- Demand prediction
- Retail analytics

## Dataset Description

### Input Dataset
File: `cleaned_retail_data.csv`

Key Columns:
- `date` – Transaction date
- `store_type` – Urban / Rural / Semi-Urban
- `product_category` – Electronics, Grocery, Clothing, Furniture
- `region` – North, South, East, West
- `brand` – Product brand
- `sales` – Units sold
- `inventory` – Stock available
- `price` – Product price
- `discount` – Discount applied


##  Tools & Libraries Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- VS Code
- Jupyter Notebook
- GitHub


##  Feature Engineering Steps Implemented

### Data Loading
- Loaded cleaned dataset from Task 1
- Verified data types and structure


###  Categorical Encoding
Applied appropriate encoding strategies:
- Label Encoding
  - `store_type`
  - `region`
  - `brand`
- **One-Hot Encoding**
  - `product_category`
  - `season`

Reasoning:
- Prevents ordinal bias
- Makes data compatible with ML algorithms


###  Scaling & Normalization
Numerical features scaled using **StandardScaler**:
- `sales`
- `inventory`
- `price`
- `discount`
- Rolling averages
- Elasticity & impact features

Purpose:
- Ensures equal contribution of features
- Improves model convergence


###  Time-Based Feature Engineering
Extracted meaningful temporal features:
- Year
- Month
- Week
- Weekday
- Quarter
- Weekend flag
- Season (Winter, Summer, Monsoon, Autumn)

These features capture **seasonality and customer behavior patterns**.


###  Retail Domain-Specific Features
Created business-driven features:
- **Rolling 7-day sales average**
- **Rolling 30-day sales average**
- **Discount impact**
- **Price elasticity indicator**

These features help models understand:
- Demand trends
- Promotional effectiveness
- Pricing sensitivity

###  Correlation Analysis & Feature Selection
- Generated correlation matrix
- Removed highly correlated features (threshold > 0.85)
- Reduced multicollinearity to improve model stability


###  Final Dataset Export
- Removed non-ML columns
- Exported final dataset as:

`engineered_retail_data.csv`

This dataset is fully ML-ready

## Output Files

| File Name | Description |
|---------|------------|
| cleaned_retail_data.csv | Cleaned input dataset |
| Task3_Feature_Engineering.ipynb | Feature engineering notebook |
| engineered_retail_data.csv | Final engineered dataset |

---

## Key Learnings
- Importance of feature engineering in ML performance
- Correct encoding strategy selection
- Handling scale sensitivity in models
- Time-series feature creation
- Domain-driven feature design
- Multicollinearity reduction


##  Next Steps
This engineered dataset can now be used for:
- Regression models
- Sales forecasting
- Demand prediction
- PCA & clustering
- Model evaluation & deployment


# Author

# SAMUEL 
Feature Engineering & Data Science Project  
Implemented using Python & VS Code

