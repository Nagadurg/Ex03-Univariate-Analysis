# Ex03-Univariate-Analysis
### Aim
To read the given data and perform the univariate analysis with different types of plots.

#### Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm
## Step1
Read the given data.

## Step2
Get the information about the data.

## Step3
Remove the null values from the data.

## Step4
Mention the datatypes from the data.

## Step5
Count the values from the data.

## Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program
Developed by :Chevula.Nagadurga
Registration Number : 212221230014
```
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
### Output
DATA



![output](./3.1.png)






DATA HEAD



![output](./3.2.png)




DATA INFORMATION



![output](./3.3.png)




DATA DESCRIBE



![output](./3.4.png)



DATA NULL VALUES





![output](./3.5.png)






DATA'S DATATYPES





![output](./3.6.png)




DATA'S VALUECOUNT





![output](./3.7.png)




BOXPLOT




![output](./3.8.png)





COUNTPLOT



![output](./3.9.png)





DISTRIBUTIONPLOT





![output](./3.10.png)





HISTOGRAMPLOT





![output](./3.11.png)






### Result
Thus we have read given data and performed the univariate analysis with different types of plots.









