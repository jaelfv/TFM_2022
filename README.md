# Demand modelling and prediction in retail

Demand forecasting is an indispensable process in the retail industry, since it leads the way to better decision-making for companies. Our main goal is to be able to predict the demand for calculating the optimal price that maximises revenue. 

Within this study we compare the results obtained after applying two different machine learning proposals to a case study with real data from a retail company.   First, a hypothesis-driven approach where we use a custom model that incorporates econometric knowledge. For that, we combine machine learning methods with a double-logarithmic demand model:



![image](https://user-images.githubusercontent.com/72398948/176197832-ca4cdb28-9b20-4da9-8ef5-f68f5a14f2d2.png)

For that, we first built a demand prediction algorithm that tries to fit the historical data provided into a double-logarithmic model where demand has a strong dependence on the price. 

Second, a data-driven approach where we use gradient boosting on decision trees to predict demand. CatBoost is used and compared to tools that are currently used in the industry based on linear regressions.

Apart from prediction activities, we also revise our results trying to find the optimal price through optimization. The study allows us to reveal the advantages of gradient boosting on decision trees over our custom model, as well as its limitations during the optimization part.

The [Report](https://github.com/jaelfv/TFM_2022/blob/main/Demand_modelling_and_prediction_in_retail.pdf) related to this study can be found in pdf format. 

## Implemented tricks and techniques
Within this study we have used several techniques and tricks:
- Moving Average variable transformation
- Lag variable transformation
- Sinus and cosinus trasnformation for periodic temporal variable as week of the year.
- GridSearch
- Time series Clustering
- Seasonal decomposition
- Autograd
- Gradient Descent
- Custom made loss function based on conditions
- CatBoost
- Python statsmodels



## Notebooks
- [Data_cleaning_H](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/Data_cleaning_H.ipynb): Contains the code for cleaning the H dataset, the analysis and the clustering study performed.
- [Dataset merge](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/DatasetMerge.ipynb): Merge of the H dataset with the Google trends datasets.
- [Basic Custom Model](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/Basic%20Custom%20Model.ipynb): Contains the Basic Model.
- [Enhanced Custom Model](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/Enhanced%20Custom%20Model.ipynb): Contains the final FAM and Enhanced learning method.
- [Visualization_loss_model](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/Visualization_loss_model.ipynb): Notebook for displaying results from Custom Model.
- [CATBOOST_CustomModel](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/CATBOOST_CustomModel.ipynb): Comparison of Custom Model with CatBoost for ShoeCare products.
- [CATBOOST_ROVA_GTX](): Comparison of CatBoost and linear regression for Womans Goretex
- [Explainability_CatBoost](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/Explainability_CatBoost.ipynb): Section where we study the explainbility for CatBoost.
- [DemandMatrix](https://github.com/jaelfv/TFM_2022/blob/main/Notebooks/DemandMatrix.ipynb): Demand matrix checks for CatBoost and FAM.


## BibTex reference format for citation for the Code
```
@misc{TFMjf,
title={Demand modelling and prediction in retail},
url={https://github.com/jaelfv/TFM_2022},
note={GitHub repository with a collection of Jupyter notebooks with relevant code used.},
author={Jael Freixanet},
  year={2022}
}

```
## BibTex reference format for citation for the report of the Master's Thesis
```
@misc{TMFjfReport,
title={Demand modelling and prediction in retail},
url={https://github.com/jaelfv/TFM_2022/blob/main/Demand_modelling_and_prediction_in_retail.pdf},
note={Report of the Master's Thesis: Demand modelling and prediction in retail},
author={Jael Freixanet},
  year={2022}
}

```
This work has been done by Jael Freixanet supervised by Jerónimo Hernández as part of the Thesis for the Master: Fundamental Principles of Data Science from Universitat de Barcelona. 
