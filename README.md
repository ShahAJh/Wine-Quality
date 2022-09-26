# Wine Quality Prediction

## NON-TECHNICAL EXPLANATION OF YOUR PROJECT

To predict human wine taste preferences using wine quality dataset. A large dataset when compared to other studies in this domain is considered, with white and red vinho verde samples from Portugal. Using preprocessing methods to process the data, after that we have tried various classification approaches using machine learning and deep learning techniques. The deep learning sequential model achieved promising results with 77.92% validation accuracy , outperforming the other classifiers. The result of this work is important for the wine industry. Furthermore, similar techniques can help in target marketing by modeling consumer tastes from niche markets.

## DATA

From the UCI Machine Learning Repository, this dataset can be used for regression modelling and classification tasks. This dataset is much larger than others available as benchmarks in the same domain, it includes info about the chemical properties of different types of wine and how they relate to overall quality. This dataset is related to red and white variants of the Portuguese "Vinho Verde" wine, launched on Date 07-10-2009. The wine data used in this study comes from the north-west region, named Minho, of Portugal. Each one of the 6407 wine samples was evaluated by a minimum of three sensory assessors, by means of blind tastes, which graded the wine in a scale that ranges from 0 to 10, that matches very bad to excellent quality, respectively. The data were collected from May 2004 to February 2007. The attribute of dataset are: type, Fixed acidity, Volatile acidity, Citric acid, Residual sugar, Chlorides, Free sulfur dioxide, Total sulfur dioxide, Density, PH, Sulphates, Alcohol Output variable (based on sensory data) and Quality (score between 0 and 10).
Wine quality dataset citation:
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis.
Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

## MODEL 

For training and testing set, we splitted the dataset train size to 80% that is equal to 5197 rows of dataset and test size of 20%  that is equal to 1300. This split method randomly splits the sample data into the testing set and the training set, so this will avoid the unseen division of the sample data.
Trying various classification approaches using machine learning k nearest neighbor, XGB classifier, logistic regression, support vector classifier and deep learning sequential model. The deep learning sequential model achieved promising results with 75% validation accuracy , outperforming the other classifiers. As sequential model is appropriate for a plain stack of layers, this means that every layer has an input and output attribute. These attributes can be used to do neat things, like quickly creating a model that extracts the outputs of all intermediate layers in a Sequential model, that's why sequential model is prefered in such scenarios.

## HYPERPARAMETER OPTIMSATION

 For the selection of optimal values, which would generate the best model output. We have used hyperparameter optimizer which is adam optimizer, it moves within the grid in a random fashion to find the best set of hyperparameters, as it goes through only a fixed number of hyperparameter settings This approach reduces unnecessary computation. By evaluating model on different values setting of epochs, batch size and adam optimizers values to get the optimum result.

## RESULTS

The results are based on test data set which were splitted 20% of randomly from an original wine quality datasets. By trying various classification approaches using machine learning and deep learning techniques. The deep learning sequential model achieved promising results  with 77.92% validation accuracy and validation score of 0.17 , outperforming the other classifiers. The proposed deep learning sequential approach is based on the model could also be used to improve the training. Furthermore, the relative importance of the inputs
brought interesting insights regarding the impact of the analytical tests. The result of this work is important for the wine industry. 


