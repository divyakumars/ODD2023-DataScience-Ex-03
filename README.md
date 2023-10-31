# ODD2023-DataScience-Ex-03
# EX-03 UNIVARIATE ANALYSIS
### Aim:
To read the given data and perform the univariate analysis with different types of plots.

### Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
### Step1: 
Read the given data.
### Step2:
Get the information about the data.
### Step3:
Remove the null values from the data.
### Step4:
Mention the datatypes from the data.
### Step5:
Count the values from the data.
### Step6:
Do plots like boxplots,countplot,distribution plot,histogram plot.
### Program:
```
Developed By: DIVYA K
Register Number: 212222230035
```

```
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
df=pd.read_csv("/content/iris (1).csv")
df.head()
df.tail()
```
CATEGORICAL DATA
```
df.nunique()
df.iloc[:,4].value_counts()
for i in range(0,df.shape[1]):
print("-----------",df.columns[i],"------------")
print(df.iloc[:,i].value_counts())
print("---------------------------------------")
sns.countplot(x='species',data=df)
```
UNIVARIATE ANALYSIS
```
dfv=df.loc[df['species']=='virginica']
plt.plot(dfv['sepal_length'],np.zeros_like(dfv['sepal_length']),'*')
plt.xlabel('sepal length')
plt.show()
##plt.plot(df_setosa['sepal_length'],np.zeros_like(df_setosa['sepal_length']),'o')
dfs=df.loc[df['species']=='setosa']
dfc=df.loc[df['species']=='versicolor']
plt.plot(dfs['sepal_length'],np.zeros_like(dfs['sepal_length']),'*')
plt.plot(dfc['sepal_length'],np.zeros_like(dfc['sepal_length']),'X')
plt.plot(dfv['sepal_length'],np.zeros_like(dfv['sepal_length']),'o')
plt.plot(dfs['sepal_length'],np.zeros_like(dfs['sepal_length']),'+')
plt.plot(dfc['sepal_length'],np.zeros_like(dfc['sepal_length']),'-')
plt.xlabel('SEPALLENGTH')
plt.show()
```
### OUTPUT:



![273362600-0fe65207-2db4-400c-9fdc-4b3556aa8181](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/58e4bf7a-cbf5-463a-9693-08a3ea4f7d81)

![image](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/b4b1f84d-5bdf-4496-93d6-6ae26d720970)


![image](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/56580360-1e6f-4294-b8af-a8839a750a9d)



![273362613-c45ae394-135a-4f07-be51-da2c8ea52300](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/4aa118e5-fe78-4b84-a704-4e998f5274a0)


![273362629-d658eef2-404f-4d84-939e-a5d5e5eb7f66](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/02d68bc0-5884-420c-871e-fc37dbe6eb44)

![273362653-04dc02fe-44fd-468b-a3b9-af9c25aa0988](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/3aa6e1d5-62e9-411f-82b3-4c5f2d1ec978)


![273362675-37d2358d-fa77-4212-8e51-ba4aa4b5e8bd](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/af6cc161-0027-4781-901a-2fa242ecc2a3)

![273362708-205f0ac7-faa2-48f4-9a44-bedd79085339](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/ac88737c-db89-4ec6-bbfd-5ade3aac5d35)

![273362737-481a483b-4aba-4dd8-9d16-d3df865dbc69](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/557ab247-4bf3-45c4-8898-d0d00e6be0d4)

![273362762-52ee5e48-9acf-4a40-955d-12819d0d0071](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/f61aa2e4-3c9b-4b56-af57-f71099e967af)


![273362800-89f5ae9e-5403-4184-bffe-23f3316a8e0c](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/d0f922a9-0a6e-47a0-a1ab-939f6bfd9568)
![273391390-79b63223-dd97-4b5e-8ce0-2128a0b7792b](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/bdd79f2b-def1-4a9d-8c83-965913ad6a38)
![273391402-2d3c3ddd-3228-4267-bd1e-790e07516e25](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/f200ca23-9c71-4340-a293-a3b1eec0109d)
![273391479-dfc91d7a-90ee-4e21-a8ed-67349dd03a28](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/db9c531c-c65b-4d14-9b4c-e3ce3593098c)
![273391497-7d85424d-19cc-4759-80d3-fbed617983d4](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/2c1d575d-c110-4858-ae93-5af38128b288)
![273391532-dc2255f6-9344-4344-9783-5f8722baadfa](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/2c14ee38-c8e3-4f6f-9c54-98cf80749d5c)

![273391554-3fcdd602-5283-45d3-a9f8-1600757c2186](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/d5e35a20-5f77-44cc-8346-fdde0471e429)

![image](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/44dc9f30-8da7-41bf-8232-afe8f445ac14)


![image](https://github.com/divyakumars/ODD2023-DataScience-Ex-03/assets/119393621/33172817-9a26-4b07-a77c-80b8c77fedf4)


### RESULT:
Hence the univariate analysis is verified.




























