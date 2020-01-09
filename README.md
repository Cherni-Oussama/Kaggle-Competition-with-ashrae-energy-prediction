# Kaggle-Competition-with-ashrae-energy-prediction


Python Jupyter Notebook with **Convolutional Neural Network** implemented in **Keras**. 

It's [Google Colab] ready.

Part of the [Kaggle competition].

Submitted Kernel with 0.995 score.

# Data (379 MB)
****
## Data Sources: 
* [building_metadata]
* [weather_test] 
* [weather_train] 
* [train] 
 * [test]
 
**Training:** 16.1M (0.8) samples

**Validation:** 4M (0.2) samples

**Testing:** 41M samples


# Model
*****
```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
lstm_1 (LSTM)                (None, None, 128)         70656     
_________________________________________________________________
dropout_1 (Dropout)          (None, None, 128)         0         
_________________________________________________________________
batch_normalization_1 (Batch (None, None, 128)         512       
_________________________________________________________________
lstm_2 (LSTM)                (None, 128)               131584    
_________________________________________________________________
batch_normalization_2 (Batch (None, 128)               512       
_________________________________________________________________
dropout_2 (Dropout)          (None, 128)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 1)                 129       
=================================================================
Total params: 203,393
Trainable params: 202,881
Non-trainable params: 512
_________________________________________________________________
```



# Training
*****
![alt text](https://imgur.com/GeydLj4.png)

# MSE Score
****
![alt text](https://i.imgur.com/B6vPMGR.png)






[building_metadata]: <https://www.kaggle.com/c/ashrae-energy-prediction/download/oFn989xw1CkkukIrkW7y%2Fversions%2FL8dMWiDsow7DMdQzNLHL%2Ffiles%2Fbuilding_metadata.csv>
[weather_test]: <https://www.kaggle.com/c/ashrae-energy-prediction/download/oFn989xw1CkkukIrkW7y%2Fversions%2FL8dMWiDsow7DMdQzNLHL%2Ffiles%2Fweather_test.csv>
[weather_train]: <https://www.kaggle.com/c/ashrae-energy-prediction/download/oFn989xw1CkkukIrkW7y%2Fversions%2FL8dMWiDsow7DMdQzNLHL%2Ffiles%2Fweather_train.csv>
[train]:<https://www.kaggle.com/c/ashrae-energy-prediction/download/oFn989xw1CkkukIrkW7y%2Fversions%2FL8dMWiDsow7DMdQzNLHL%2Ffiles%2Ftrain.csv>
[test]:<https://www.kaggle.com/c/ashrae-energy-prediction/download/oFn989xw1CkkukIrkW7y%2Fversions%2FL8dMWiDsow7DMdQzNLHL%2Ffiles%2Ftest.csv>
[Google Colab]: <https://colab.research.google.com/>
[Kaggle competition]: <https://www.kaggle.com/c/ashrae-energy-prediction>
