# Model Card

## Model Description

**Input:** 

This dataset has the 12 fundamental features input with 6497 samples which are responsible for affecting the quality of the wine. The inputs of dataset are: type, Fixed acidity, Volatile acidity, Citric acid, Residual sugar, Chlorides, Free sulfur dioxide, Total sulfur dioxide, Density, PH, Sulphates, Alcohol Output variable (based on sensory data).

**Output:** 

To predict human wine taste preferences the target feature is quality. The quality feature in a scale that ranges from 0 to 10, that matches very bad to excellent quality, respectively.  Consisdering this project as binary classification problem, by converting the quality feature into zeros and ones using data segregation to create a separate two different groups of classes.

**Model Architecture:** 

_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 48)                528       
                                                                 
 dense_1 (Dense)             (None, 36)                1764      
                                                                 
 dense_2 (Dense)             (None, 24)                888       
                                                                 
 dense_3 (Dense)             (None, 8)                 200       
                                                                 
 dense_4 (Dense)             (None, 1)                 9         
                                                                 
=================================================================

Total params: 3,389
Trainable params: 3,389
Non-trainable params: 0

_________________________________________________________________


## Performance

The performance of model are based on test dataset which were splitted 20% of randomly from an original wine quality datasets. The deep learning sequential model achieved promising results with 77.92% validation accuracy and validation score of 0.17 , outperforming the other classifiers.

## Limitations

Keras's sequential model is not capable to handle low-level computations. This  model  may present limited learning capabilities, complex models may overfit the data, losing the capability to generalize, sequential model has hyperparameters that need to be adjusted, such as the number of hidden nodes or, in order to get good predictive accuracy. While being more flexible models, the performance depends on a correct setting of hyperparameters, therefore adjustment of hyperparater must be relative. 

## Trade-offs

Its trade offs is that, in order to get reliable results, training usually have to be run over a long stretch of time. This time requirement could decrease through the usage of parallel or distributed computing system. Keras's sequential model is not capable to handle low-level computations. Therefore, it runs on the top of TensorFlow, Theano, and Microsoft CNTK.
