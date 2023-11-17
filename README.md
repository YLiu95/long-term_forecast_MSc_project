# MSc project: Use Large Artificial Neural Nets to Extract Semantic Signals for Long-term Sequential Forecasting
## multi-step (30-days) forecast the price of sterling in Chinese yuan

[repository on GitHub](https://github.com/YLiu95/multi-step_forecast_MSc_project)

creater: [Yishan Liu](https://www.linkedin.com/in/yl95/)

## introduction

- this is a collection of the materials I used for my MSc proejct on long term financial time series forecasting with deep learning.
- this collection includes the data I used, my paper, and my python implementaiton.
- I am looking forward for your feedbacks, thank you!

## compare 5 RNN encoder-decoders and their non encoder-decoder versions
- the 5 RNN encoder-decoders are:
   1. GRU encoder-decoder
   2. bidirectional GRU encoder-decoder
   3. CNN-GRU encoder-decoder
   4. convLSTM encoder-decoder
   5. **bidirectional convLSTM encoder-decoder** (**I created this new architecture**)

$${\color{red} **bidirectional \space convLSTM \space encoder-decoder**}$$

- the 5 non encoder-decoders are:
   1. GRU
   2. bidirectional GRU
   3. CNN-GRU
   4. convLSTM
   5. bidirectoinal convLSTM

## visualised result from the best performing model:
forecasting result from bidirectional GRU encoder-decoder:
![bidirectional gru forecasting result](https://user-images.githubusercontent.com/82934216/190156726-e5898a0f-f0d8-42bf-8c70-f411d7687b19.png)
- evaluation metrics:
    - train mse: 0.0361340157687664 
    - test mse:  0.017722204327583313 
    - train rmse: 0.17656706273555756 
    - test rmse:  0.12243817746639252

- other statistics - means:
    - training data mean:    8.841544827586207 
    - train prediction mean: 8.791829 
    - testing data mean:     8.717213409961685 
    - test prediction mean:  8.674898 

- other statistics - standard deviations:
    - training data standard deviation:    0.17639548961572413 
    - train prediction standard deviation: 0.0813758 
    - testing data standard deviation:     0.14175250034034664 
    - test prediction standard deviation:  0.06592484
