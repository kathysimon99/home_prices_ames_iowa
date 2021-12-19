


# Problem Statement:
Use a variety of features of a housing marking to provide a model that will predict the price of buying a house. As a home buyer or someone is interested in flipping houses it is important to be able to create an accurate sales price for the house. The model that is created will be a great resource to accurately predict the selling price of the home.

## Background Information
The data was collected from the Ames Assessor’s Office about individual residential properties sold in Ames, Iowa from 2006 to 2010. There are 82 features, including numerical and categorical.

The data sets can be found on the [Kaggle.](https://www.kaggle.com/c/dsi-920-ames/data)

## Data Dictionary
Data description can be found at [DataDocumentation.txt](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)
The data dictionary below includes changes that were made to the original data

|Feature|Type|Dataset|Description|
|---|---|---|---|
|year_built         |int |https://www.kaggle.com/c/dsi-920-ames/data |calculated age of house from 2010
|year_remod/add     |int |https://www.kaggle.com/c/dsi-920-ames/data |calculated age of renovation
|kitchen_qual       |int |https://www.kaggle.com/c/dsi-920-ames/data |used the following mapping 'Ex': 5, 'Gd': 4, 'TA': 3, 'Fa': 2, 'Po': 1
|neighborhood       |int |https://www.kaggle.com/c/dsi-920-ames/data |Created 3 groups of neighborhoods based on average sales price, top 25% : 5, middle 50%: 3, bottom 25%:1


### Summary of Analysis
I included features that had a strong linear correlation to create a linear regression model. The base on the R2 scores for the training and testing data, the model was underfitting the data. Using polynomial features, I created a more complex linear model, that when regularized by LASSO fit the data better. The 

### Conclusions
- Overall quality and kitchen quality appeared to add the most value to the home.
- Improve the overall quality and kitchen quality of the home to increase the value.
- Recommended neighborhoods for investment:
  * Stone Brook ⬩Northridge Heights ⬩ Northridge ⬩Green Hills ⬩Veenker Timberland ⬩Somerset ⬩Clear Creek
- Future recommendations 
  * Further analysis with tax data, economy and interest rates
