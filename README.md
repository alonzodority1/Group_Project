
=======

# An Analysis of Grain Merchandising In Relation To Futures Contracts
=======
#### Application of Machine Learning to Predict a Competitive Agriculture Commodity Purchase and Procurement Strategy for Food Manufactures
##### by Alonzo Dority, Chris Barton, Jaime Chusid, Shola Thompson

![Grain Commodities.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/550eb83b8236335d1ba9cd62392c8a9106767391/Grain%20Commodities.png)

## Overview of Project
Food manufactures face a lot of pressure to keep costs stable and maintain a competitive advantage or reduce costs to increase profits. Hence, Food Manufacturers have to be skilled at purchasing commodities at the optimal price. Using artificial neural systems increases the possibility to progress Food Manufacturers ability to reliably process information needed to determine whether to purchase a commodity based on criteria that makes it an ideal purchase price. Agricultural commodity goods, like Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn are raw materials that are integral to the production of many food manufacturers’ end product. Therefore the purpose of this project is to create a predictive model for Food Manufacturers to inform when is the best time to purchase. It is well documented that agricultural commodities are sensitive to market variability through exchange rates, interest rates, and the supply and demand of the global economy. Therefore, the creation of a predictive model for purchasing and procurement will allow food manufacturers to effectively predict, negotiate, purchase and procure raw materials at the best possible price.

#### Background of this project
On average, agricultural commodities account for 55 cents of every dollar spent to manufacture the end product within the Food and Beverage Manufacturing industry. With such a high cost ratio, it is imperative that manufactures know the right price to buy raw materials. Purchasing agricultural commodities too high will result in grave financial impacts. 
Further, the continuing impact of COVID-19, has resulted in reduction in demand, thus resulting in a higher cost derived from increased volume of inventory and storage of unsold end products. In this challenging environment, food manufactures are being forced to rethink the way they purchase and procure agricultural  raw materials. 
This project aims to develop a predictive model to guide food manufacturers in the purchase of agricultural commodities during the COVID-19 climate and beyond.

#### Purpose of this project
The purpose of the project is to utilize Artificial Neural Network (ANN) modeling to transforming the way food manufacturing companies manage the risk associated with purchasing agricultural raw materials/commodities. 
Specifically, this project aims to utilize ANN modeling to inform Food manufacturers when to purchase Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn based on the price of the commodity at proposed purchase time point. The model will use a time series analysis to ascertain whether the commodity meets the threshold of cost price 5% lower than 90 days prior. If the commodity cost price indicated is 5% lower than 90 days prior, the recommendation would be to purchase. The model would be considered effective if the model is correct 70% of the time.

#### Dataset
Data source was derived from Yahoo APIs, historical stock data for Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn commodities from 2006 to present. Data consisted of historical commodity futures, foreign exchange and U.S. interest rate pricing data from March 2006 – present.
![Yahoo Finance.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/ebba517c2b38261a60c6cd0daa9c7d7681360493/Yahoo%20Finance.png)

###### Limitations Of The Dataset
Historical prices for Chinese yen FX rate not included for all commodities, due to inability to find open-source data.

## Analysis Plan
1. Analyze and investigate the applications of ANN across all food manufacturing agricultural commodities (Sugar, Soybean Oil, Soybeans, Wheat, Cotton and Corn) purchasing 
2. Find the suitability of the type of ANN in various domains of food manufacturing purchasing
3. Use of deep learning in purchasing agricultural commodities and how they relate across commodities, 
4. Find the importance in applicability and real use of ANN research in a decade’s worth of historical pricing data for all commodities since 2006 
5. Investigate challenges of future use of model
#### 3 Main Questions we Aim to Answer:
1. Which commodity pricing is able to most accurately predict the others?
2. How do pricing fluctuations of one commodity predict pricing of the others?
3. How do we determine whether to buy these commodities or wait?

## Analysis
First data frames were created with historical pricing and measures of central tendency for each commodity. Next we ran a  multiple linear regression to determine which commodity has the most dependency on the other variables. Then we split data into testing and training sets to prepare for machine learning model.
#### Artificial Neural Network (ANN)
The ANN model was designed to make a decision to buy a select commodity in the present or hold and purchase at a later date . The model will use a time series analysis to ascertain whether the commodity meets the threshold of cost price 5% lower than 90 days prior. If the commodity cost price indicated is 5% lower than 3 months prior, the recommendation would be to buy. 

![Analysis Phase.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/dd4840b0321ec4a2c86767cdc9f04f30e8ab0b73/Analysis%20Phase.png)

As the graphic above indicates, thirty-three (33) features were created, and data was encoded, then divided using train test split. Data was scaled and then fed to the neural network. The neural network is comprised of a sequential model and consists of two hidden layers and an output layer. The first layer consists of 80 nodes, while the second layer consists of 30 nodes. The output layer consists of one node. Activation functions include ReLu, ReLu, and sigmoid, respectively. The neural network was then compiled using a binary crossentropy loss function, an Adam optimizer, and uses accuracy as the metric. The ANN analysis is designed to make a binary classification. The model is trained using 100 iterations to consistently achieves approximately 70% accuracy. 

#### Use of Technology
![Technologies Used.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/2a744f2f8c5434d785b291e12876fae406042e0a/Technologies%20Used.png)

The analysis was conducted using a number of technologies. Analysis was primarily performed in python using a Jupyter notebook. Data was retrieved from a mongodb and loaded into a notebook with pandas. Results were acquired using an artificial neural network with the tensor flow platform. All data was then uploaded into our GitHub repository. In addition, the analysis used other platforms, including Tableau, scikit-learn, Matplotlib, and Yahoo Finance

## Presentation of Findings
Figure 1: Buy vs. Hold
The table below illustrates the first 4 rows of the Buy Vs Hold model for Corn. The model is trained to return "BUY" when cost price is 5% lower than cost 90-days prior and "Hold" when cost price is 5% higher than cost 90-days prior.

![Buy vs Hold Corn.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/553040d5d947e919f9babb642eb04bce2aa09b98/Buy%20vs%20Hold%20Corn.png)

Figure 2: Predictability of Models per Commodity
ThE analysis was repeated 6 times, once for each commodity. The table below indicates the respective accuracy scores. All models achieved around 60-70% accuracy. The predictability of the models varied per commodity as expected, with the strongest results being in Soybeans and Soy Oil.

![Model Accuracy by Commodity.png](https://github.com/sholathompson/https-github.com-alonzodority1-Group_Project/blob/553040d5d947e919f9babb642eb04bce2aa09b98/Model%20Accuracy%20by%20Commodity.png)

## Limitations of Study: 

#### Recommendations for Future Analysis
Our first recommendation for a future analysis is to include Japan's currency, the Yen. The Yen ranks third as the world’s most used currency, behind the U.S. dollar and Euro, which we have included in our analysis. However, we were unable to access open-source historical stock data for Yen currency.
Second, the model can be adjusted to predict pricing for a commodity, rather than making a buy or hold decision. With the time constraints of this project, we did not believe this was feasible, but could be done in the future.
Lastly, we recommend including external factors such as climate or time of year. These factors could provide more insight into the changing stock prices. Our model used data from 90 days prior to make a present-day decision instead we could have looked further back than that, to make a buy or hold decision. Looking at the time of year and patterns that may have occurred in prior years may offer more insight into the future stock prices of the commodities.

## Future Research
Research shows a link between crude oil prices and agricultural commodities price indexes.  Future work should include historical stock data from Crude Oil to examine price influence among the crude oil and raw materials in the model. 



