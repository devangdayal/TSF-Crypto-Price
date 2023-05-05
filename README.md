# SUPERVISED DEEP LEARNING APPROACH FOR TIME SERIES FORECASTING ON CRYPTOCURRENCY ASSET PRICES

## DEVELOPMENT FLOW AND PHASES OF IMPLEMENTATION

The development flow and phases of implementation of the project is shown below :

<div align="center">
  <img  src="Project Images/Dev Flow .png" alt="devflow"></img>
</div>


## Data Visualisation

### Weight Distribution Plot

<p> The Bar plot shows Bitcoin, Ethereum, and Cardano are the three most popular crypto currencies for trading or investment.This type of chart is useful for visualizing the weight distribution of different cryptocurrencies in a clear and concise manner. The color-coding of the bars makes it easy to quickly identify the most heavily weighted cryptocurrencies, and the sorting by weight makes it easy to see which cryptocurrencies are most important in the overall portfolio. </p>
<div align="center">
<img width="800" alt="image" src="https://user-images.githubusercontent.com/53809748/236430865-f25aafbe-1bbd-4888-bed9-f54732458eda.png">
</div>

### Correlation Plot 

From the Correlation plot below, we can see Bitcoin Cash is highly correlated with EOS.IO. Binance Coin is correlated with many crypto currencies, such as , Bitcoin, Bitcoin Cash, Cardano, Ethereum
  
<div align="center">
<img width="610" alt="image" src="https://user-images.githubusercontent.com/53809748/236431092-29b83639-9534-4bb9-90ef-32b8dc023702.png">
</div>

From the Correlation plot shown below, we can see correlation between the attributes and target variable. It shows that the `Open`, `High`, `Low`, `Close`, and `VWAP` are highly correlated.

<div align="center">
<img width="775" alt="image" src="https://user-images.githubusercontent.com/53809748/236431282-87fa4ba8-bc4c-4c71-bf59-4296336bc09b.png">
</div>

### Price Trends in Years

We will use the Closing Price and Candlestick graph as shown in Figure below to capture the trends of the crypto currency. We can see there is tremendous price increase for BTC, ETH, and ADA in 2021, which implies they are all good investment.

<div align="center">
  
![image](https://user-images.githubusercontent.com/53809748/236431556-dafffd2a-0655-4e5c-80be-f034587700c2.png)
  
</div>

As we can see in figure below ETH, and BTC residual returns are relatively stable compared to ADA. This might be a good implication that if the investor would take short time trading opportunities, ADA is a better choice. If the investor is risk averse, BTC or ETH will be a better fit.

<div align="center">
  
![image](https://user-images.githubusercontent.com/53809748/236431685-dd7d9ca1-0610-4fc7-81bb-4ebad8d18d54.png)
  
</div>


### Scatter Plot for the Attributes

<div align="center">
  
![image](https://user-images.githubusercontent.com/53809748/236431804-33237a17-fa53-4d77-8ff6-960350ab841e.png)
  
</div>

### Candlestick Chart

Candlestick charts are a type of financial chart used to represent price movements in financial markets, such as stocks, currencies, and commodities. They are called "candlestick" charts because they resemble a series of candlesticks with wicks on top and bottom representing the high and low prices, and a body representing the opening and closing prices of a given time period. 

<div align="center">
<img width="751" alt="image" src="https://user-images.githubusercontent.com/53809748/236432042-3aa9b176-8516-4c4b-8162-512e1135aeba.png">

<img width="751" alt="image" src="https://user-images.githubusercontent.com/53809748/236432311-66417dfb-a9d2-4c37-a12f-43de13fed42e.png">
</div>

### Seasonal Decomposition

Seasonal decomposition is a method to break down a time series into its trend, seasonal and residual components. This method helps in understanding the underlying patterns and structures of the time series, which is useful for forecasting and decision-making.

<div align="center">
  
![image](https://user-images.githubusercontent.com/53809748/236432581-5d6be998-e9dc-4a10-98d4-cdd660354d86.png)
  
![image](https://user-images.githubusercontent.com/53809748/236432628-0cf619cf-8016-470e-9333-b2b062109c6a.png)
  
</div>

### Box-Cox Transformation

Box-Cox transformation is a method used to transform non-normal dependent variables into a normal shape. It is used to stabilize the variance, make the data confirm more closely to normality, and improve the fit of the data to statistical models.
<div align="center">
<img width="766" alt="image" src="https://user-images.githubusercontent.com/53809748/236432770-fc522f7c-3c8b-45cb-9dd6-6aba8815efff.png">

![image](https://user-images.githubusercontent.com/53809748/236432825-085fb1e3-67e7-4d0b-87f3-27f249f88054.png)
</div>

## Model Trained on the Dataset

- Random Forest

Random Forest is a popular machine learning algorithm that can be used for time series forecasting. In the context of time series forecasting, Random Forest can be used as a regression algorithm.
To use Random Forest for time series forecasting, we first need to create a feature matrix that consists of lagged variables. The lagged variables can be created using the shift() function in pandas.

- XGBoost (Gradient Boost)

Gradient Boosting is a popular machine learning technique used for time series forecasting, particularly when the data has a complex relationship between the input and target variables. It involves fitting a sequence of models, each of which is trained to predict the difference between the target variable and the previous model's prediction. These predictions are then added to the previous model's predictions, creating an ensemble model that improves over time.

- ARIMA Model

The ARIMA model is a popular time series model that combines autoregressive (AR), differencing (I), and moving average (MA) components. AR models use past values of a time series to predict future values, while MA models use past forecast errors. The I component is used to make the time series stationary. ARIMA models are used to make short-term forecasts and are particularly useful when the time series exhibits trends, seasonality, and/or autocorrelation.

- LSTM RNN

LSTM networks use a memory cell that can selectively forget or store information over time, allowing the network to remember information from earlier in the sequence and use it to make predictions. This makes them particularly useful for tasks such as language translation and speech recognition.
GRUs are a simpler variant of LSTM networks that use fewer parameters, making them faster to train and more memory-efficient. They also have fewer gates, making them more straightforward to implement and interpret.


- LSTM RNN - Attention Mechanism 

Attention Mechanism is a key innovation in the field of deep learning, which has been successfully applied in various natural language processing (NLP) and computer vision (CV) tasks. It is a method that allows neural networks to selectively focus on certain parts of the input sequence while ignoring others. Attention mechanisms are especially useful in situations where the input sequence is long and complex, such as in machine translation, text summarization, and image captioning.
The idea of attention can be understood through an example. Suppose we are translating a sentence from English to French. If the sentence is very long, it might be difficult for the neural network to keep track of all the relevant information at once. Instead, the network can selectively focus on different parts of the input sentence, one at a time.


## Conclusion and Result 

Based on the Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) results obtained from different models, we can infer their relative performance in predicting the target variable. A lower MSE and RMSE indicate better predictive accuracy of the model, while higher values indicate lower accuracy.
For instance, in the given case, the LSTM - Attention Mechanism model has the lowest MSE and RMSE values of 0.00280 and 0.0529, respectively, compared to the other models. This implies that the LSTM-Attention model has the highest predictive accuracy and is the most reliable in forecasting the target variable.
On the other hand, the Random Forest and Gradient Boost models have relatively higher MSE and RMSE values compared to the other models, indicating lower predictive accuracy. The ARIMAX and LSTM-RNN models also have lower MSE and RMSE values than the Random Forest and Gradient Boost models but higher than the LSTM-Attention model. Hence, we can infer that the LSTM-Attention model performs the best in predicting the target variable among all the models tested.

<div align="center">
<img width="600" alt="image" src="https://user-images.githubusercontent.com/53809748/236433745-18edd1e2-a6bf-44ab-88f2-b5e1640d9248.png">
  
</div>
