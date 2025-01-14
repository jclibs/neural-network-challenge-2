# neural-network-challenge-2

In this project a tensorflow keras model is used to predict Attrition and Department from a dataset, using data from ten selected columns.

```
selected_cols = ['Education','Age', 'DistanceFromHome', 'JobSatisfaction', 'OverTime', 'StockOptionLevel',
                 'WorkLifeBalance', 'YearsAtCompany','YearsSinceLastPromotion', 'NumCompaniesWorked']
```

In the X data the 'OverTime' column is changed to numeric values using a map function, and the rest of the columns are scaled using the standard scaler. Then the Y features are both encoded using OneHotEncoder.

Next the keras model is made using an input layer, three shared layers, and one hidden and one output layer for both Attrition and Department. The model is then compiled and tested.

The attrition accuracy of the model is 0.79891, and the department accuracy is 0.5163.