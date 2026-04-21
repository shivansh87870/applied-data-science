## Task Day 12

Phase: Pandas
Focus Area: Transformation
Problem Statement: Convert categorical columns into numeric using encoding.

Solution:
```python
import pandas as pd

df = pd.DataFrame({
    'City': ['Delhi', 'Mumbai', 'Delhi', 'Chennai'],
    'Gender': ['Male', 'Female', 'Female', 'Male']
})

 Label Encoding
df['Gender_encoded'] = df['Gender'].map({'Male': 1, 'Female': 0})

One-Hot Encoding
df_encoded = pd.get_dummies(df, columns=['City'])

print(df_encoded)
```

Output:
```
     Gender  Gender_encoded  City_Chennai  City_Delhi  City_Mumbai
0      Male               1             0           1            0
1    Female               0             0           0            1
2    Female               0             0           1            0
3      Male               1             1           0            0
```
## Task Day 13

Phase: Pandas
Focus Area: GroupBy
Problem Statement: Analyze total sales per region using groupby.

Solution:
```python
import pandas as pd

data = {
    'Region': ['North', 'South', 'North', 'East', 'South'],
    'Sales': [100, 200, 150, 300, 250]
}

df = pd.DataFrame(data)

region_sales = df.groupby('Region')['Sales'].sum()
print(region_sales)
```
Output:
```
Region
East     300
North    250
South    450
Name: Sales, dtype: int64
```
## Task Day 14

Phase: Pandas
Focus Area: Mini Task (Data Cleaning)
Problem Statement: Clean and preprocess a raw dataset.

Solution:
```python
import pandas as pd

df = pd.DataFrame({
    'Name': ['A', 'B', None],
    'Age': [25, None, 30],
    'Salary': [50000, 60000, None]
})

Fill missing values
df['Age'].fillna(df['Age'].mean(), inplace=True)
df['Salary'].fillna(df['Salary'].median(), inplace=True)

Drop rows with missing Name
df.dropna(subset=['Name'], inplace=True)

print(df)
```
Output:
```
  Name   Age   Salary
0    A  25.0  50000.0
1    B  27.5  60000.0
```
## Task Day 15

Phase: Visualization
Focus Area: Matplotlib
Problem Statement: Plot monthly sales trend using line chart.

Solution:
```python
import matplotlib.pyplot as plt

months = ['Jan', 'Feb', 'Mar', 'Apr']
sales = [200, 300, 250, 400]

plt.plot(months, sales, marker='o')
plt.title('Monthly Sales Trend')
plt.xlabel('Months')
plt.ylabel('Sales')
plt.show()
```
Output:
```
Displays a line chart showing monthly sales trend
```
## Task Day 16

Phase: Visualization
Focus Area: Seaborn
Problem Statement: Visualize distribution of exam scores using histogram.

Solution:
```python
import seaborn as sns
import matplotlib.pyplot as plt

scores = [50, 60, 70, 80, 90, 75, 85, 65]

sns.histplot(scores, bins=5, kde=True)
plt.title('Distribution of Exam Scores')
plt.show()
```
Output:
```
Displays histogram showing distribution of scores
```
### Challenge Overview

These tasks focus on applying Pandas and visualization libraries to real-world data scenarios, including data transformation, aggregation, cleaning, and visual analysis. The exercises help in understanding how raw data is converted into meaningful insights through structured workflows.

Skills Practiced
Data transformation and encoding techniques
Handling categorical variables
Data aggregation using GroupBy
Data cleaning and preprocessing
Handling missing values using statistical methods
Data visualization using Matplotlib and Seaborn
Understanding trends and data distributions
Writing clean and structured Python code
Submission

Completed independently and implemented structured solutions for each task. Practiced real-world data preprocessing, analysis, and visualization techniques essential for data analytics roles.

Turning raw data into meaningful insights is the foundation of every data-driven decision.
