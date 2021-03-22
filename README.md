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
- [Neural Network](https://github.com/ChrisBarton107/Group_Project/blob/main/Group%20NeuroNetwork.ipynb)
- Stock/financial data was used. The model is designed to make a decision to buy a select commodity in the present or hold and purchase at a later date.<br>
- There are currently 33 features. Data is encoded, then divided using train test split. It is topped off by scaling the data, then fed to the neural network. The neural network is a sequential model and consists of two hidden layers and an output layer. The first layer consists of 80 nodes, while the second layer consists of 30 nodes. The output layer consists of one node. Activation functions include ReLu, ReLu, and sigmoid, respectively. The neural network is then compiled using a binary crossentropy loss function, an Adam optimizer, and uses accuracy as the metric.<br>
- We decided to extract different data from our analysis, so our machine learning model is very different than the model used previously. We previously attempted to perform a regression analysis but have adjusted the analysis and designed the neural network to make a binary classification. The model is trained using 100 iterations and consistently achieves approximately 70% accuracy. With an accuracy score like this, the model performs well but needs to be optimized and improved if it is to be used in an industrial setting.<br>


###### Dataset
###### Limitations Of The Dataset
## Presentation of Findings
## Limitations Of Study
## Future Work
