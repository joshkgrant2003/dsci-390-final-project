# DSCI 390: Supervised Machine Learning - Final Project

This project focuses on building a predictive model to estimate the resale prices of motorcycles using a dataset containing key features such as `age`, `mileage`, `engine_size`, and `brand`. This project was developed using the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework, which ensured a structured and thorough approach to data analysis.

## Project Overview

- **Goal:** Accurately predict the resale prices of motorcycles to aid businesses and individuals in making informed decisions.
- **Data:** Contains features such as:
    - `name`: Motorcycle Name
    - `selling_price`: Selling Price of Motorcycle
    - `year`: Year of Vehicle
    - `seller_type`: Individual or Dealer
    - `owner`: 1st, 2nd, 3rd, or 4th Owner
    - `km_driven`: Kilometers Driven on Motorcycle
    - `ex_showroom_price`: Price of Vehicle at Auction
- **Framework:** CRISP-DM, consisting of six stages:
    - *Business Understanding*
    - *Data Understanding*
    - *Data Preparation*
    - *Modeling*
    - *Evaluation*
    - *Deployment*

## Project Structure

#### `Data` Folder

This folder contains the datasets used throughout this project. The `Motorcycles.txt` file was the file given to us by our instructor. The `Motorcycles.csv` file was created from the `.txt` file. This file just simply removed the headers at the top of the file. The `abt_motorcycle_prices.csv` file is the dataset we use to train the models in this project. This dataset contains extra features aquired through **feature engineering**, and it also removed missing values and outliers. The stages of building and curating this dataset are performed in the `FinalProject_DataQualityReport.ipynb` file in the `Deliverables` folder.

#### `Deliverables` Folder

This folder contains all the deliverables for the project that were submitted to our instructor. This includes:
    - `FinalProject_DataQualityReport.ipynb`: file containing python code that analyzes and cleans the dataset, as well as creating our own features through feature engineering.
    - `FinalProject_Modeling.ipynb`: file containing python code that builds two different machine learning models (linear regression and random forest regression) using `scikit-learn`. It also uses `matplotlib` and `seaborn` for building visualizations to help learn more about the data and the model. 
    - ***Business Use Case Synopsis - Joshua Grant.docx***: file containing a write-up and summary of the project and its findings. 
    - ***Visualizations - Joshua Grant.docx***: file containing visualizations from the code that act as handouts for a client if we were to present this case in a boardroom setting. 

#### `Documentation` Folder

This folder contains word documents from earlier in the semester that contain more information about the **Business Understanding**, **Data Understanding**, and **Data Preparation** stages of the CRISP-DM process. They delve a little deeper and more in-depth into the context behind this project and the plans leading up to everything you see in the `Deliverables` folder.

#### `Visualizations` Folder
This folder contains `.png` files of the same visualizations created in the jupyter notebook files mentioned earlier.

## Key Features

- **Exploratory Data Analysis:**
    - Visualized data distributions and relationships between features.
    - Highlighted key trends and insigts, such as the correlation between ex-showroom price and resale price.
- **Feature Engineering:**
    - Added derived features such as `age`, `usage_intensity`, and `brand`.
    - Addressed missing and inconsistent data for robust model training.
- **Model Development:**
    - Applied **Random Forest Regression** for its interpretability and performance
    - Utilized *hyperparameter tuning* using `GridSearchCV` to enhance model accuracy.
- **Model Performance:**
    - Achieved high accuracy with minimal residuals between actual and predicted values.

## Visualizations

1. **Feature Importance:**
    - Identifies key drivers for resale price prediction.
2. **Actual vs. Predicted Prices:**
    - Demonstrates model performance, with predictions closely aligned with actual resale prices.
3. **Residual Distribution**:
    - Aids in identifying if errors are randomly distributed or showing some sort of pattern.

## Usage

- Python 3.12+
- Jupyter Notebook
- Libraries Used:
    - `pandas`
    - `numpy`
    - `matplotlib`
    - `seaborn`
    - `scikit-learn`

## License

This project is licensed under the MIT license. See the `LICENSE` file for details.