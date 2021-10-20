# Fraym.io
Fraym.io~Mini_Data_Case_Part_1 : Please feel to reach out to me at sreyadha@buffalo.edu if the notebook file does not load properly; I can email you the notebook.

All the plots including plots from Plotly and Folium could be visible in the below link:
https://colab.research.google.com/drive/18XSsC8d9n1_FqsC2FyKXGXurjobAjE10

# Interpretation of the Models


The current dataset contains more than 500 locations in  Nigeria to predict the median expenditure of several Nigerian neighborhoods. To explore the rastar data, locations have been plotted in folium and plotly library to have an overview on how the expenditure is correlated with other predictor variables. Data exploration has been carried out from several relationship plots in seaborn library to establish a few general trends in data observations. Standard procedures in feature engineering (lasso regression, random forest regressor) and outlier removal (Quantile rule: mean +/- 3std) have been carried out as the final step of data preprocessing. Min-max normalization has been applied only on the predictor variables. Since the response variable is very skewed, it has been barred from any data normalization. The dataset has been split into 75:25 for train and test sets. The overall prediction scores are moderately suitable for both the sets from polynomial regression,  Support vector machine (polynomial kernel), Decision tree, and k-nearest neighbor (k=3) algorithms. Otherwise, the tree-based models like RandomForest, XGBoost, and Adaboost algorithm predictions on train and test sets are better. It has been established that if proper hyperparameter tuning could be carried out on a tree-based model like XGBoost, the prediction could give an accuracy score on a test set of as high as 57%, which is 9.4% higher than the accuracy metric from the best KNN model.  

Based on the current analysis to predict median expenditure, tree-based models outperformed regression analysis to minimize the test set's generalization error. **If I had to choose one model for prediction, I would go for XGBoost with the best hyper-parameters because once the model is hyper tuned, its the most favorable for forecasts. We might need to compromise on execution time, though.**




