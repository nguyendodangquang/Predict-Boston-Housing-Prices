# Predict-Boston-Housing-Prices
Predicting Boston Housing prices In this project with different Traditional Machine Learning model (LinearRegression, KNeighborsRegressor). Included evaluating the performance and predictive power of my model on data collected from homes in suburbs of Boston, Massachusetts.
## Dataset
The dataset for this project originates from the UCI Machine Learning Repository. The Boston housing data was collected in 1978 and each of the 506 entries represent aggregated data about 14 features for homes from various suburbs in Boston, Massachusetts Data preprocessing has been applied to the dataset. For the purposes of this project, the following preprocessing steps have been made to the dataset:

- 16 data points have an 'MEDV' value of 50.0. These data points likely contain missing or censored values and have been removed.
- 1 data point has an 'RM' value of 8.78. This data point can be considered an outlier and has been removed.
- The features 'RM', 'LSTAT', 'PTRATIO', and 'MEDV' are essential. The remaining non-relevant features have been excluded.
- The feature 'MEDV' has been multiplicatively scaled to account for 35 years of market inflation.
## Model
KNeighborsRegressor and Linear Regression
## Discussion
- KNN is working better since it is more flexible since we don't make an assumption about our f(x) (that our features have linear relationships)

- The fact that the data was collected in 1978 makes this data set less relevant to today-market. Inflation plays an important role here as many factors in society, economy and market have changed which results in the difference in house prices. Hence, using this data set to predict current house prices will only be good for reference

- Though the 3 features we have here are important in determining the price of a house, it is insufficient. There are many other factors that may influence the price, for example, the condition of the house or of the appliances, the availibility of extra things like pools, garages,...

- As our model only has 3 features and not that complex, it may not be consistent in prediction if we putting in some odd cases. And obviously a model that is trained with urban dataset would be insufficient to apply to rural areas because of the differences in their characteristics. Those characteristics in a sense would decide the influential degree of different features in the 2 kinds of areas.

- In my opinion, it is not fair to judge the price of a house based only on its surroundings (neighborhood). These features certainly are important and have big influences on the price, but there are other features that may play an important role as well.
