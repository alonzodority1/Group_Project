# An Analysis of Grain Merchandising In Relation To COVID19 and Futures Contracts

[Google Slides Presentation](https://docs.google.com/presentation/d/1lX-Z_V_9o-AszHN1m9Lmd9607_SnTwXcho3M-1k3lOM/edit#slide=id.p) 

## Overview of Project
To make informed decisions, grain merchandisers need to predict the future price of commodities based on their current price. As more grain merchandisers create future contacts with buyers as a strategy to minimize risk, knowing whether to accept or reject a given price, becomes increasingly important.
###### Background of this project 
Demand of grain merchandise has been severely impacted as consumer behavior has significantly decreased due to COVID19. As COVID19 pandemic continues to thwart the supply chain and reduce demand due consumer underspending, it is important to support grain merchandisers with predictive tools to leverage the uncertainty of the COVID19 climate. 
Research suggests that grain producers experience higher costs and lower revenues as a result of COVID-19 with the Food and Agricultural Policy Research Institute at the University of Missouri projecting a $21.9 billion decrease in farm income in 2021.
###### Purpose of this project
This project aims to support grain merchandisers with identifying possible opportunities for profit by using Artificial Neural Network (ANN) algorithms, time series methods such as seasonal ARIMA and State Space models, and other approaches to identify relationships overtime in the cash price of Soybean, Corn, Cotton and Wheat. 
This project aims to develop a structural model to explain COVID-19 merchandising behavior as compared to pre-COVID-19, and forecast performance of these commodities within the COVID-19 climate and beyond.

###### Neural Network Model
- Stock/financial data was used. High and Low data were dropped while Close and Volume data were kept. Range data was created by subtracting Low data from High data prior to dropping High and Low data.<br>
- There are currently 23 features, including Close, Volume, and Range data for seven categories, including Corn, Wheat, Cotton, Crude, USDBRL, EURUSD, and IR. Features also include Volume and Range data for Soybeans.<br>
- Close data for Soybeans is used as our target, or y. Data is encoded, then divided using train test split. It is topped off by scaling the data, then fed to the neural network.<br>
- Our model is still incomplete as we are deciding how we want to bin data. We are also experimenting with several loss and activation functions in effort to find the optimal components for a regression analysis. Because the model is incomplete, it’s unclear as to how the model is limited and how we benefit from using it in our analysis.<br>
- [Neural Network](https://github.com/ChrisBarton107/Group_Project/blob/main/NeuralNet_PriceData.ipynb)<br>
## Analysis Plan
###### Dataset
###### Limitations Of The Dataset
## Presentation of Findings
## Limitations Of Study
## Future Work
