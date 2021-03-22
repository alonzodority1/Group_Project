# Application of Machine Learning to Predict a Competitive Agriculture Commodity Purchase and Procurement Strategies for Food Manufactures
## Overview of Project
Food manufactures face a lot of pressure to keep costs stable to maintain a competitive advantage or reduce costs to increase profits. Hence, Food Manufacturers have to be skilled at purchasing commodities at the optimal price by forecasting the cost price of commodity goods to decide whether to buy or not. Agricultural commodity goods, like Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn are raw materials that are integral to the production of many food manufacturers’ end product. Therefor the purpose of this project is to create a predictive model for Food Manufacturers to inform when is the best time to purchase. It is well documented that agricultural commodities are sensitive to market variability through exchange rates, interest rates, and the supply and demand of the global economy. Therefore, the creation of a predictive model for purchasing and procurement will allow food manufacturers to effectively predict, negotiate, purchase and procure raw materials at the best possible price.
###### Background of this project
On average, agricultural commodities account for 55 cents of every dollar spent to manufacture the end product within the Food and Beverage Manufacturing industry. With such a high ratio, it is imperative that manufactures know the right price to buy raw materials. Purchasing agricultural commodities too high will result in grave financial impacts. 
Further, the continuing impact of COVID-19, has resulted in reduction in demand, thus resulting in a higher cost derived from increased volume of inventory and storage of unsold end products. In this challenging environment, food manufactures are being forced to rethink the way they purchase and procure agricultural  raw materials. 

This project aims to develop a predictive model to guide food manufacturers in the purchase of agricultural commodities during the COVID-19 climate and beyond.


###### Purpose of this project
The purpose of the project is to utilize Artificial Neural Network (ANN) modeling to transforming the way food manufacturing companies manage the risk associated with purchasing agricultural raw materials/commodities. 
Specifically, this project aims to utilize ANN model to inform Food manufacturers when to purchase Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn based on the price of the commodity at proposed purchase time point. The model will use a time series analysis to ascertain whether the commodity meets the threshold of cost price 5% lower than 3 months prior. If the commodity cost price indicated is 5% lower than 3 months prior, the recommendation would be to purchase. The model would be considered effective if the model is correct 70% of the time.
#### Dataset
Data source was derived from Yahoo APIs, historical stock data for Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn commodities from 2006 to present.
#### Limitations Of The Dataset
Historical prices for Chinese yen FX rate not included for all commodities, due to inability to find open-source data.
#### Analysis Plan
1. Analyze and investigate the applications of ANN across all food manufacturing agricultural commodities (Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn) purchasing 
2. Find the suitability of the type of ANN in various domains of food manufacturing purchasing
3. Use of deep learning in purchasing agricultural commodities and how they relate across commodities, 
4. Find the importance in applicability and real use of ANN research in a decade’s worth of historical pricing data for all commodities since 2006 
5. investigate challenges of future use of model

## Analysis
First data frames were created with historical pricing and measures of central tendency for each commodity. Next we ran a  multiple linear regression to determine which commodity has the most dependency on the other variables. Then we split data into testing and training sets to prepare for machine learning model.

#### Artificial Neural Network (ANN)
The ANN model was designed to make a decision to buy a select commodity in the present or hold and purchase at a later date . The model will use a time series analysis to ascertain whether the commodity meets the threshold of cost price 5% lower than 90 days prior. If the commodity cost price indicated is 5% lower than 3 months prior, the recommendation would be to buy. 

Thirty-three (33) features were created and data was encoded, then divided using train test split. Data was scaled and then fed to the neural network. The neural network is comprised of a sequential model and consists of two hidden layers and an output layer. The first layer consists of 80 nodes, while the second layer consists of 30 nodes. The output layer consists of one node. Activation functions include ReLu, ReLu, and sigmoid, respectively. The neural network was then compiled using a binary crossentropy loss function, an Adam optimizer, and uses accuracy as the metric.

The ANN analysis is designed to make a binary classification. The model is trained using 100 iterations to consistently achieves approximately 70% accuracy. 
## Presentation of Findings
Figure 1: Commodity pricing by year

Figure 2: Historical pricing data - buy vs. hold

Figure 3: The Average cost of Agricultural costs for Food manufacturing 2006 to present

Figure 4: Commodity pricing relationships 

Table 1: RMSE, MAE and R2 calculated for the training and test sets for each predictive model.
 		 	 	 	 
Figure 5: Scatter plot of the relationship between the input weight and the Commodities cost price. Outliers identified according to the 1.5*IQR rule are marked in red. The solid line is a model fitted using local polynomial regression.

Figure 6: Crude oil vs. the six commodities (cotton, corn, soy, wheat, soy oil, sugar)

Figure 7: Pre-Covid vs. post-Covid

## Limitations Of Study
The model performs well but needs to be optimized and improved if it is to be used in an industrial setting.
## Future Work

