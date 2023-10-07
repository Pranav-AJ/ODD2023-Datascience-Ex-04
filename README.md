# ODD2023-Datascience-Ex-04

## AIM

To perform multivariate analysis on a dataset.

## ALGORITHM

1. Import the necessary libraries.
2. Read the data.
3. Perform data cleaning process.
4. Visualize and analyse the data using various plots.

## CODE AND OUTPUT
```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```
```
df=pd.read_csv("/content/iris (1).csv")
df.head()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/a1bb0e4f-8c5b-4557-8f01-8957ce387d10)
```
df.tail()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/eaefc4da-0d95-45e1-abc4-9684f851f8ac)

```
sns.FacetGrid(df,hue="species").map(plt.scatter,"petal_width","sepal_width").add_legend();
plt.show()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/f1e4db50-086b-4075-a377-3ca5e3741da8)

```
sns.FacetGrid(df,hue="species").map(plt.scatter,"petal_length","sepal_length").add_legend();
plt.show()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/af5168c5-f3e0-482b-9bb3-ef2b72a83969)

```
sns.FacetGrid(df,hue="species").map(plt.scatter,"petal_length","sepal_length").add_legend();
plt.show()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/ab12044d-1cd6-4cb7-9401-e59fefa97e70)

```
sns.pairplot(df,hue="species",size=3)
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/c9bf9f4f-39ca-4ee6-b489-cfa654bee808)

```
df.nunique()
```
![image](https://github.com/Pranav-AJ/ODD2023-Datascience-Ex-04/assets/118904526/477bdf00-6a90-48dd-83f7-c89abf2c0379)
