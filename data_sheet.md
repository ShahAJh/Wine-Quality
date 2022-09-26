# Datasheet Template

## Motivation

In recent years, the interest in wine has increased, leading to growth of the wine industry. As a consequence, companies are investing in new technologies to improve wine production and selling. The main aim of this project was to develop an approach to predict human wine taste preferences and also to determine wheather can we or not accurately predict the quality of wine based off some of its chemical properties and features. These approaches can help in target marketing by modeling consumer tastes from niche markets. 
The dataset was created by P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis and it is openly available from the UCI machine learning repository (UCI, 2015).
 
## Composition

The data in the usual csv format where we have 12 feature columns and a single target column. The whole dataset has numerical values except for one column “type” which indicates the wine type like white or red. This dataset has the 12 fundamental features with 6497 samples which are responsible for affecting the quality of the wine. Wine quality  dataset contains 38 missing values.
Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.). The classes in datasets are ordered but not balanced (e.g. there are much more normal wines than excellent or poor ones).

## Collection process

The data were collected from May 2004 to February 2007. This dataset is much larger than others available as benchmarks in the same domain. There are 4898 observations of white wine and 1599 observations of red wine each frame with 13 variables giving us a 6497 by 13 dataframe. Each one of the 6407 wine samples was evaluated by a minimum of three sensory assessors, by means of blind tastes, which graded the wine in a scale that ranges from 0 to 10, that matches very bad to excellent quality, respectively. Each expert graded the wine quality between 0 (very bad) and 10 (very excellent). Below, I see that the bulk of the wine quality is at a quality of 5, 6 and 7. There are no observations below a quality of 3 and none above 9. The final score is given by the median of these evaluations, which corresponds to the output variable. This target variable denotes a typical normal shape distribution, with minimum and maximum values of 3 and 9 for the red and white wine.

## Preprocessing/cleaning/labelling

It is quite impossible to process the data having ‘NaN’ with it and so replacing nan values by mean of individual features respecively.
Taking it as a classification model converting the quality feature into zeros and ones using data segregation to create a separate two different groups of classes. In machine learning, higly corelated features leads to decreased generalization performance on the test set due to high variance and less model interpretability as in heat map we can conclude that the ‘total sulphur dioxide’ is highly correlated features so, we will drop this feature.
Using MinMaxScaler preprocessing technique on the dataset to scales all the data features in the range [0, 1] or else in the range [-1, 1]. This scaling compresses all the inliers in the narrow range [0, 0.005]. Converting “type” features which indicates the wine type like white or red as it is acategorical data type will replace it with the numerical data 0 and 1.

## Uses

Wine certification prevents the illegal adulteration of wines (to safeguard human health) and assures quality for the wine market. Quality evaluation is often part of the certification process and it can be used to improve wine making (by identifying the most influential factors) and to statisfy wines such as premium brands (useful for setting prices). Similar techniques can help in target marketing by modeling consumer tastes from niche markets.
Each 6407 wine samples was evaluated by a minimum of three sensory assessors, by means of blind tastes, that pretty much sums as this data is unbiased but the classes in datasets are ordered but not balanced (e.g. there are much more normal wines than excellent or poor ones) and it contains 38 missing values. 

## Distribution

The whole dataset has numerical values except for one column “type” which indicates the wine type like white or red. This dataset has the 12 fundamental features with 6497 samples which are responsible for affecting the quality of the wine. There are 4898 observations of white wine and 1599 observations of red wine each frame with 13 variables giving us a 6497 by 13 dataframe. The classes in datasets are ordered but not balanced (e.g. there are much more normal wines than excellent or poor ones).
Wine quality is open dataset mainly used for research purposes. Wine quality dataset citation:
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis.
Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

## Maintenance

The data were collected from May/2004 to February/2007 using only protected designation of origin samples. Since last collected sample feb 2007 no other entries have been further included in this dataset. Dataset was launched on Date 07-10-2009, this dataset is openly available from the UCI machine learning repository (UCI, 2015).
