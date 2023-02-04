# Predicting Sales of a Major Grocery Store Chain
Christian Palisoc

Using various data analytics methods on this partuclar data set, we will help the retailer understand the properties of products and outlets that play crucial roles in increasing sales.

## Data Source
link to dataset: https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view  
original source: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

## Data Dictionary
![Data Dictionary](https://github.com/cipalisoc/project1/blob/main/project%20data%20dictionary.png)

# After the data was cleaned, the following were performed:
## Exploratory Data Analysis
A histogram and boxplot were implemented during the exploratory data analysis phase to illustrate the relationship between various categorical and numerical columns

![MRP_vis](https://github.com/cipalisoc/project1/blob/main/MRP_vis(1).png)
- This historgram illustrates the number of low fat and regular fat products among the various ranges of MRP offered

![Boxplot](https://github.com/cipalisoc/project1/blob/main/Outle%20loc_vis.png)
- This boxplot shows the distribution of item outlet sales for the three different Outlet Location Types

## Explanatory Data Analysis
- To illustrate the data for explanatory purposes, two barplots were implemented
- The barplots were chosen to show wherethe most sales were highlighted along with the display area of the products

![itemtype](https://github.com/cipalisoc/project1/blob/main/sales%20by%20type_vis.png)
- The barplot shows the number of sales by item type with Household Goods, Fruits and Vegetables, and Snacks as the top three items with the most sales.

![Area](https://github.com/cipalisoc/project1/blob/main/area%20display_vis.png)
- This barplot shows the item visibility percentage of the item types.
- The top three items with the most visibility exposure are Canned goods, Household goods, and Friuts and Vegetables

## Machine Learning Models
To predict future sales, linear regression and regression tree models were implemented with a focus on the Root Mean Squared Error (RMSE) and R-Squared Score (R2). The target variable was "Item_Outlet_Sales"

## Linear Regression Results
- Training Set
    - RMSE: 1139.1029909446283
    - R2 score: 0.5615559908552253
- Test Set
    - RMSE: 1092.8656236965487
    - R2 score: 0.5671021734263202

## Regression Tree Results
- Training Set
    - RMSE: 5.50728349323243e-15
    - R2: 1.0
- Testing Set
    - RMSE: 1493.27512593923
    - R2: 0.19177638337083347

Between the two models, the linear regression model fared better than the decision tree model. The decition tree model's results had a high variance, hence a training R2 score of 100% and a low test score of 19%. This is also a reflection in the disparity in the training RMSE between the two models. Although the linear regression model made more sense, it wasn't necessarily a good R2 score and can be improved with further tuning

## Conclusion and Recommendations
After running the data through the two models, it is clear that the linear regression model provided a better fit. Tuning of the model is definitely recommended for an optimal R2 score including modeling the data with a Decision Forest and a bagged tree model to obtain potentially better results.  

## Limitations and Next Steps
Model implementation should not be limited to these two models. Further tuning and modeling should be considered to ensure the best possible result before forecasting sales. This should also include simplifying the dataset to elimiate the high variance demonstrated in the regression tree model. Since the project is limited to these two models, all parameters of the decision tree model should be tuned alongside the consideration of the MSE and MAE. 

## Inquiries, Further Information
Contact Christian Palisoc  
cipalisoc@gmail.com

