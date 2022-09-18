# natty-storage-price-model
Attempt to create some model to predict US & EU Natural Gas Storage and NG Futures Price
I've tried to use Prophet to predict US & EU Nat Gas Storage, the model seems working good for the US NG Storage meanwhile is not performing good with the EU storage prediction.
For the US Futures Price prediction (very difficult to do) I used from sklearn.tree import DecisionTreeRegressor. This prediction is very difficult to perform since the price of the Future contracts aren affected from several variables to consider:
- US overall Storage
- Weather Conditions in terms of HDD (heating degree days) and CDD (cooling degree days)
- LNG export
- US daily Nat Gas production in Bcf
- Event (Black Swan): pipeline explosion, wars, hurricane etc...

All the data are public from:
investing.com
yahoo.finance
agsi+
EIA 
