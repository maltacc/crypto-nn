# Cryptocurrency Buy/Sell Predictor
A recurrent neural network to predict whether to buy or sell 4 cryptocurrencies using only historical data. I selected the LSTM model, which achieved a 55% accuracy score. 

# Data & Data Cleaning
* The historical data of 4 cryptocurrencies were used to train the buy/sell classifier
* Method: If the price of the crypto increased after 3 days, crypto would be bought. Otherwise it would be sold. 
* To prevent undersampling of 'buy' currencies, I implemented SMOTE to produce balanced sample data sets by generating synthetic samples

# Model 
* The binary classifier used an LSTM model with sparse categorical crossentropy for the loss function and an SGD optimizer. 

# Limitations
* The model was trained using only historical prices when in reality many factors influence the price of a stock, including media and government regulations. This accounts for some of the error. The predictor could be improved upon by drawing from recent news, deploying the model, or testing multiple models using the Lazy Classifier. 
