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
