# Importingt the Libraries!
```
# importing the libraries related to the data manipulation.
import numpy as np
import pandas as pd

# importing the libraries related to the data_visualization
import seaborn as sns
import matplotlib.pyplot as plt
%matplotlib inline
```

# Loading the Dataset!
```
df = pd.read_excel(r'...\....\python\airData_Train.xlsx')
df.head()
```
```
df.shape
```

# Data Cleaning 

```
df.isnull().sum()
```
```
df.dropna(inplace=True)
```
```
df.info()
```

# Handling the categorical data present in the dataset

We are using 2 main Encoding Techniques to convert Categorical data into some numerical format
```
1. `Nominal data` --> data are not in any order --> `OneHotEncoder` is used in this case
   
2. `Ordinal data` --> data are in order --> `LabelEncoder` is used in this case
```

# Airline vs Price Analysis :

![Image of airline vs price](https://github.com/samarth3557/Flight-Fare-Prediction-using-ML-model/blob/main/Images/Airline%20vs%20price.png)

From graph we can see that ```Jet Airways``` Business have the highest Price., Apart from the first Airline almost all are having similar median

# Outlier :

![Image of outliers](https://github.com/samarth3557/Flight-Fare-Prediction-using-ML-model/blob/main/Images/outliers.png)

# Training the Machine Learning Model!
## Linear Regression Model :
```
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn import metrics
```

![Image of LinearRegression](https://github.com/samarth3557/Flight-Fare-Prediction-using-ML-model/blob/main/Images/LinearRegression.png)

Hence using the linear regression model we have obtained an ```accuracy of 77% which is not upto the mark```. Hence we can improve this accuracy by considering another 
```Machine Learning models such as the Random Forest Model, Decision Tree model``` etc.

## RandomForest Regression :
```
from sklearn.model_selection import train_test_split
from sklearn import metrics
from sklearn.ensemble import RandomForestRegressor
```

![Image of RandomforestRegression](https://github.com/samarth3557/Flight-Fare-Prediction-using-ML-model/blob/main/Images/RandomForest%20Regression.png)

Hence we can see that the ```RandomForest Model achieved an accuracy of 87%``` which is good as compared to our previous model that is linear regression model.

# Conclusion :
   This complete notebook represents an exploratory data analysis (EDA) process to put together the patterns related to the Flight fare prediction. We have dealt with the flight fare data ```airData_Train.xlsx``` and grouped only a single column that is with the ```price``` feature. The purpose of this study is to analyze the dataset and obtain important insights form it. As visual representations are flexible and easy to understand, the results or outputs produced in the form of graphs can help people comprehend the current situation insights easily. The dataset used may not be an updated version; hence the inferences may vary from time to time as graphs can be generated as the data increases. As the amount of data increases, the trends may change and lead to different inferences and solutions. Hence we considered two different Machine learning models, the accuracy of the ```LinearRegression model``` was around ```77%``` which was not upto the mark. So we decided to use the ```RandomForest Regressor model``` which led to a very good accuracy of ```87 Percent``` which is a pretty cool accuracy for an Machine Learning Model.
   

## Thank you!!






