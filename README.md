# Smart Thermostat Project

**Project Description**: To create the prototype for the smart thermostat that can be 
switched on/off based on information about family members behavior: departure or arrival time, 
temperature at home at the same timestamps, geolocations, distance out of home and time to reach home.


## Table of Contents
- [Dataset creation, generation of synthetic data](dataset_sample_thermostat.ipynb)
- [EDA and Modeling](Prototype_EDA_Modeling.ipynb)

## Installation
This project does not require any specific installation steps. It mainly consists of CSV files and Jupyter notebooks, which can be directly accessed and opened.

To view and interact with the notebooks, you will need to have Jupyter Notebook or JupyterLab installed on your local machine. If you don't have it installed, you can follow the official Jupyter documentation to install it: [Jupyter Installation Guide](https://jupyter.org/install).

Once you have Jupyter installed, you can simply clone or download this repository and open the Jupyter notebooks (*.ipynb) in the Jupyter interface to explore the project. Also you need to save these csv files at the same directory where notebooks are.

In addition, you need to have installed Python and the next libraries: **pandas, numpy, Datetime, PCA, math, geopy, seaborn, Matplotlib.pyplot, Scipy, Sklearn, Statsmodels.api, xgboost, joblib**


## Usage
In terms of the project 2 notebooks were created, where you can find 4 key steps:
- **Data creation**: 
  - synthetic data for family with 4 members for 2022
  - feature engineering 
- **Exploratory data analysis**
- **Visualization of relationships between variables**
- **Modeling principals**:
  -Data split: train - 60%, validation - 20%, test - 20%
  - Focused metrics: F1-Score 
  (F1-Score was chosen as a key metric because saving money is important 
  as well as comfortable temperature at home)
  - Principal Component analysis (PCA=4)
  - Tuning technique: Grid Search
  - 5-fold Cross Validation

## Results
- Supervised model was created (20 variables). The target variable has 1 or 0 values and responds for swithing on/off the thermostat according to some rules
- In terms of modeling 3 models Logistic Regression, Random Forest and XG Boosting were run
- The best F1-Score was reached with XG Boosting model - 98%. 
- The most important variables were found and visualized

**Next steps**
- To train this model with different datasets 
- The final dataset looks pretty simple it means we need to improve the quality and quantity of our dataset
- To pay more attention on geolocation and motion speed


## License

[License information](LICENSE)
