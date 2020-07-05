# Toxic-Text-Classifier
A text classifier build using RNN (LSTM) to classify toxic comments  

Model Summary
Model: "sequential"
_________________________________________________________________
|Layer (type)|----------------|Output Shape|------------|Param|    
_________________________________________________________________
|embedding (Embedding)-------(None, 1403, 32)-----------160000    
_________________________________________________________________
lstm (LSTM)------------------(None, 1403, 100)----------53200     
_________________________________________________________________
flatten (Flatten)------------(None, 140300)-------------0         
_________________________________________________________________
dense (Dense)----------------(None, 64)-----------------8979264   
_________________________________________________________________
dense_1 (Dense)--------------(None, 1)------------------65        
_________________________________________________________________
Total params: 9,192,529
Trainable params: 9,192,529
Non-trainable params: 0

Kaggles Toxic Comment Challenge Dataset (https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data) was used to train this model.
TensorFlow was used to build this model

The file contains another model with more number of LSTM layers and 6 categories to classify over.

Model 2 Summary
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param    
_________________________________________________________________
embedding (Embedding)        (None, 1403, 32)          320000    
_________________________________________________________________
lstm (LSTM)                  (None, 1403, 128)         82432     
_________________________________________________________________
lstm_1 (LSTM)                (None, 256)               394240    
_________________________________________________________________
dense (Dense)                (None, 128)               32896     
_________________________________________________________________
dense_1 (Dense)              (None, 64)                8256      
_________________________________________________________________
dense_2 (Dense)              (None, 6)                 390       
_________________________________________________________________
Total params: 838,214
Trainable params: 838,214
Non-trainable params: 0
