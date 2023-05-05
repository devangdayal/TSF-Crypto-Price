# Time Series Forecasting for Cryptocurrency Asset using Long Short Term Memory with Attention Mechanism

## DEVELOPMENT FLOW AND PHASES OF IMPLEMENTATION

The development flow and phases of implementation of the project is shown below :

<div align="center">
  <img  src="Project Images/Dev Flow .png" alt="devflow"></img>
</div>


## Data Visualisation

### Weight Distribution Plot

<p> The Bar plot shows Bitcoin, Ethereum, and Cardano are the three most popular crypto currencies for trading or investment.This type of chart is useful for visualizing the weight distribution of different cryptocurrencies in a clear and concise manner. The color-coding of the bars makes it easy to quickly identify the most heavily weighted cryptocurrencies, and the sorting by weight makes it easy to see which cryptocurrencies are most important in the overall portfolio. </p>

<img width="800" alt="image" src="https://user-images.githubusercontent.com/53809748/236430865-f25aafbe-1bbd-4888-bed9-f54732458eda.png">


### Correlation Plot 

From the Correlation plot below, we can see Bitcoin Cash is highly correlated with EOS.IO. Binance Coin is correlated with many crypto currencies, such as , Bitcoin, Bitcoin Cash, Cardano, Ethereum

<img width="610" alt="image" src="https://user-images.githubusercontent.com/53809748/236431092-29b83639-9534-4bb9-90ef-32b8dc023702.png">


From the Correlation plot shown below, we can see correlation between the attributes and target variable. It shows that the `Open`, `High`, `Low`, `Close`, and `VWAP` are highly correlated.

<img width="775" alt="image" src="https://user-images.githubusercontent.com/53809748/236431282-87fa4ba8-bc4c-4c71-bf59-4296336bc09b.png">


### Price Trends in Years

We will use the Closing Price and Candlestick graph as shown in Figure below to capture the trends of the crypto currency. We can see there is tremendous price increase for BTC, ETH, and ADA in 2021, which implies they are all good investment.


![image](https://user-images.githubusercontent.com/53809748/236431556-dafffd2a-0655-4e5c-80be-f034587700c2.png)


As we can see in figure below ETH, and BTC residual returns are relatively stable compared to ADA. This might be a good implication that if the investor would take short time trading opportunities, ADA is a better choice. If the investor is risk averse, BTC or ETH will be a better fit.

![image](https://user-images.githubusercontent.com/53809748/236431685-dd7d9ca1-0610-4fc7-81bb-4ebad8d18d54.png)



### Scatter Plot for the Attributes

![image](https://user-images.githubusercontent.com/53809748/236431804-33237a17-fa53-4d77-8ff6-960350ab841e.png)



### Candlestick Chart

Candlestick charts are a type of financial chart used to represent price movements in financial markets, such as stocks, currencies, and commodities. They are called "candlestick" charts because they resemble a series of candlesticks with wicks on top and bottom representing the high and low prices, and a body representing the opening and closing prices of a given time period. 

<img width="751" alt="image" src="https://user-images.githubusercontent.com/53809748/236432042-3aa9b176-8516-4c4b-8162-512e1135aeba.png">

<img width="751" alt="image" src="https://user-images.githubusercontent.com/53809748/236432311-66417dfb-a9d2-4c37-a12f-43de13fed42e.png">


### Seasonal Decomposition

Seasonal decomposition is a method to break down a time series into its trend, seasonal and residual components. This method helps in understanding the underlying patterns and structures of the time series, which is useful for forecasting and decision-making.

![image](https://user-images.githubusercontent.com/53809748/236432581-5d6be998-e9dc-4a10-98d4-cdd660354d86.png)
![image](https://user-images.githubusercontent.com/53809748/236432628-0cf619cf-8016-470e-9333-b2b062109c6a.png)


### Box-Cox Transformation

Box-Cox transformation is a method used to transform non-normal dependent variables into a normal shape. It is used to stabilize the variance, make the data confirm more closely to normality, and improve the fit of the data to statistical models.

<img width="766" alt="image" src="https://user-images.githubusercontent.com/53809748/236432770-fc522f7c-3c8b-45cb-9dd6-6aba8815efff.png">

![image](https://user-images.githubusercontent.com/53809748/236432825-085fb1e3-67e7-4d0b-87f3-27f249f88054.png)

