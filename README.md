# Yes_bank_stock_prediction

![image](https://user-images.githubusercontent.com/95841292/202706607-372b1391-c041-40a0-8528-c51be84f60c9.png)

**In 2018 scam happened in Yesbank, because of which stock suddenly fell from Its all time high of more than  rupees 400 to rupees 150 whithin a month.**
**Yes Bank Limited is an Indian private sector bank headquartered in Mumbai, India and was founded by Rana Kapoor and Ashok Kapur in 2004. It offers wide range of differentiated products for corporate and retail customers through retail banking and asset management services. On 5 March 2020, in an attempt to avoid the collapse of the bank, which had an excessive amount of bad loans, the Reserve Bank of India (RBI) took control of it**

# 📋 Problem Satement

**Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company**
**B'coz of sudden fall in any stock, investors looses lot of money, This project will help them to understand the future performance of that stock.**
**The main objective is to predict the stock’s closing price of the month**

# 📋 Visualizations
 
Yes_bank_stock_price_trend from 2005 to 2020
![Yes_bank_stock_price_trend](https://user-images.githubusercontent.com/116551866/216925761-e2a33d14-45fe-4dbc-97c9-ca16e3d90a09.PNG)

# 1) stock price over time 
![Candle_stick_chart](https://user-images.githubusercontent.com/116551866/216926863-a369501b-3717-4e11-bb87-a5134a4a1cc4.PNG)

# 2) correlation 

![image](https://user-images.githubusercontent.com/95841292/202969499-52f1114e-00b6-4478-a459-651dbb0aa5fa.png)

# 📋 Model used-

# Linear regression
![linear_reg](https://user-images.githubusercontent.com/116551866/216928265-e650b62c-19f9-4e84-8069-ac099ca802b6.PNG)

# Lasso regression after gridsearch cv
![Lasso_Cv](https://user-images.githubusercontent.com/116551866/216928531-8bca39f8-d280-4e9a-a29c-afd9325526f3.PNG)

# Ridge regression after gridsearch cv
![Ridge_cv](https://user-images.githubusercontent.com/116551866/216928711-209435c6-c50f-46f3-8a57-cf58d7987243.PNG)

# Elasticnet regression after gridsearch cv
![Elasticnet_cv](https://user-images.githubusercontent.com/116551866/216928900-b2d2e83a-801a-473e-9bb0-7e5cd0f98b62.PNG)

# Decision tree
![DT](https://user-images.githubusercontent.com/116551866/216929098-a83abb15-02e7-476f-8c8b-3852da2212b9.PNG)

We performed Linear regression setting high, low and open as independent variables. Divided the dataset into training and testing datasets. We transformed the data using log tranformation which transforms each feature distribution Uniformly. We predicted the closing price of the test data using the Linear regression model we have trained.
Then we also used regularization and desicion tree model. Out of all desicion tree model is performed well.
We have calculated various metric like MAE, MAPE, MSE, RMSE, r2 scores for all the five models

# 📋 model performance

![performance](https://user-images.githubusercontent.com/116551866/216933679-138c987a-f6a5-4294-a5bd-9d8fb5e242d5.PNG)

# 📋 Conclusion
-  In EDA part we observed that:
1.  There is increase in trend of Yes Bank's stock's Close,Open,High,Low price till 2018.
2.  We can see that in August, stock closed near its month low. It is a sign that market is losing it's strength and may be it will go in bear phase.
3.  We observed that open vs close price graph concluded that after 2018 yes bank's stock hitted drastically.
4.  Target variable(dependent variable) strongly dependent on independent variables
5.  We get maximum accuracy of 99%
6.  Linear regression and Ridge regression get almost same R squared valueWhereas Lasso ans Elasticnet model shows lowest R squared value.
7.  Desision Tree model performed well on test data.
8.  So  Desision Tree model will we use as a final model for this project b'coz it is giving highest R2 score and explainability of Desision Tree is also goog and R2 score is the final metric we'll use to evaluate our model.

