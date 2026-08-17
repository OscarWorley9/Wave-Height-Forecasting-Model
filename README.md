**# Wave-Height-Forecasting-Model**

This project stemmed from my interest as a surfer and my curiosity on how Surfline predicts wave height.

This project compares a baseline model, Linear Regression algorithm with a Long-term Short-term memory algorithm in forecasting Brighton wave height in a 24 hour period.

**Datasets**:
https://coastalmonitoring.org/realtimedata/?chart=81&tab=download&disp_option=
https://coastalmonitoring.org/realtimedata/charts_neco/?chart=88&tab=download&disp_option=

**Linear Regression (LR)**
Linear regression is a machine learning algorithm used to predict a (continuous) outcome y, based on the value of one or more predictor variables x, by fitting a hyperplane to the data.
The reason I chose LR is it provides an interpretable statistical baseline which has a variety of graphs to visualise data which makes it easy to compare models. Making it the ideal benchmark.

**Long-term Short-Term Memory (LSTM)**
LSTM is a recurrent neural network designed to process sequential data.
The deciding factor for choosing LSTM is its ability to fix recurring neural networks vanishing gradient problem, which is perfect for a large time series forecasting.
**Results**
| Model             | R²   | MAE   | RMSE  |
|-------------------|------|-------|-------|
| Linear Regression | 0.31 | 0.40m | 0.57m |
| LSTM              | 0.65 | 0.26m | 0.40m |


**REQUIREMENTS**
pip install pandas numpy torch scikit-learn utide matplotlib seaborn optuna
