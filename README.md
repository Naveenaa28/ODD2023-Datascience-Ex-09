## Ex-09-Data-Visualization-
## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 
## Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.
## ALGORITHM
## STEP 1
Read the given Data
## STEP 2
Clean the Data Set using Data Cleaning Process
## STEP 3
Apply Feature generation and selection techniques to all the features of the data set
## STEP 4
Apply data visualization techniques to identify the patterns of the data.

## CODE
```
NAVEENAA V.R
212221220035
```
```
import seaborn as sns
import matplotlib.pyplot as plt
tips=sns.load_dataset('tips')
tips

tips.head()

tips.info()

sns.barplot(x='day',y='total_bill',data=tips)
plt.title("Weekly highest total bill amount")

sns.barplot(x='smoker',y='tip',data=tips, palette='rainbow')
plt.title("Average tip amount given by smokers and non-smokers")

sns.boxplot(x='size', y='tip',data=tips)
plt.title("Tip percentage based on the sizes of the dining party")

sns.boxplot(x='sex', y='tip',data=tips)
plt.title("Higher tips based on gender")

plt.plot(tips['day'],tips['total_bill'])
plt.title("Relationship between the total bill amount and the day of the week")
plt.show()

sns.violinplot(x='time',y='total_bill',data=tips)
plt.title("Distribution of total bill amounts vary across different time periods(lunch vs. dinner)")

sns.barplot(x='size',y='total_bill',data=tips)
plt.title("Highest average total bill amount based party size")

sns.boxplot(x='day',y='total_bill',data=tips)
plt.title("Distribution of tip amounts for each day of the week")

sns.violinplot(x='time',y='tip',data=tips)
plt.title("Tip based on the type of service ")
sns.scatterplot(data=tips, x='total_bill', y='tip')
correlation_coefficient = tips['total_bill'].corr(tips['tip'])
print("Correlation Coefficient:", correlation_coefficient)

tips.corr()
plt.subplots(figsize=(7,5))
sns.heatmap(tips.corr(),annot=True)
```


## OUTPUT
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/c1bd5162-6658-4e3b-93be-09562cdcfcdc)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/ad5ffac9-3fc2-4ee6-b7b8-3bc11f78ce20)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/09aebc85-bdf9-4233-b7cc-83c5ef74fa4f)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/939a9978-ab5f-4d31-9e57-790df98bb2bf)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/aa705d50-70fd-471e-b5db-517aa1f6a69a)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/c43cab9b-da87-4d24-b3da-ae7fcb56b664)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/eee352df-1d80-4e4c-b382-b0ee9e4c1470)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/14247d14-659e-4358-bee2-b8d2790852fb)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/72b58eed-1c0e-41d1-8cff-b803ece368eb)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/6d9658bc-b7da-458e-ab53-c806b3894b37)
![image](https://github.com/Naveenaa28/ODD2023-Datascience-Ex-09/assets/131433133/38532c0a-1d9f-4d01-ad06-3b39872bc278)
## RESULT:
Hence, Data Visualization is applied on the complex dataset using libraries like Seaborn and Matplotlib successfully based on tips dataset and the data is saved to file.
