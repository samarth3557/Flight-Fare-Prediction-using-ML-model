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

# Data Cleaning 
1. This function displays the total count of null values in each column
```
df.isnull().sum()
```
2. dropping the null values if present
```
df.dropna(inplace=True)
```
3. df.info()
```
df.info()
```

# Handling the categorical data present in the dataset
```
