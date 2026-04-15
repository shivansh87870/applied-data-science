# Python Data Science Practice — 
## Task Day 07, Day 08, Day 09, Day 10, Day 11
## Task Day 07

Phase: Python
Focus Area: Mini Task
Problem Statement: Build a student marks analysis program using lists and dictionaries.

Solution:
```python
students = {
    "Aman": [85, 90, 78],
    "Riya": [88, 76, 95],
    "Karan": [70, 80, 65]
}

for name, marks in students.items():
    total = sum(marks)
    average = total / len(marks)
    print(f"{name} -> Total: {total}, Average: {average:.2f}")
```
Output:
```
Aman -> Total: 253, Average: 84.33
Riya -> Total: 259, Average: 86.33
Karan -> Total: 215, Average: 71.67
```
## Task Day 08

Phase: Python
Focus Area: NumPy
Problem Statement: Create a NumPy array of temperatures and find min, max, and average.

Solution:
```python
import numpy as np

temps = np.array([30, 32, 35, 31, 29, 36, 33])

print("Min:", np.min(temps))
print("Max:", np.max(temps))
print("Average:", np.mean(temps))
```
Output:
```
Min: 29
Max: 36
Average: 32.28
```
## Task Day 09

Phase: NumPy
Focus Area: Matrix Ops
Problem Statement: Perform matrix addition and multiplication using NumPy.

Solution:
```python
import numpy as np

A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

print("Addition:\n", A + B)
print("Multiplication:\n", np.dot(A, B))
```
Output:
```
Addition:
[[ 6  8]
 [10 12]]

Multiplication:
[[19 22]
 [43 50]]
```
## Task Day 10

Phase: Pandas
Focus Area: DataFrames
Problem Statement: Create a DataFrame from CSV and display first 10 rows.

Solution:
```python
import pandas as pd

df = pd.read_csv("data/sample_data.csv")

print(df.head(10))
```
Output:
```
Displays first 10 rows of dataset
```
## Task Day 11

Phase: Pandas
Focus Area: Cleaning
Problem Statement: Handle missing values in a dataset using mean/median.

Solution:
```python
import pandas as pd

data = {
    "Marks": [85, None, 90, 78, None, 88]
}

df = pd.DataFrame(data)

df["Marks_mean"] = df["Marks"].fillna(df["Marks"].mean())
df["Marks_median"] = df["Marks"].fillna(df["Marks"].median())

print(df)
```
Output:
```
   Marks  Marks_mean  Marks_median
0   85.0       85.00          85.0
1    NaN       85.25          86.5
2   90.0       90.00          90.0
3   78.0       78.00          78.0
4    NaN       85.25          86.5
5   88.0       88.00          88.0
```
### Challenge Overview

These tasks focus on applying Python, NumPy, and Pandas to real-world data scenarios including data aggregation, statistical computation, matrix operations, data handling, and data cleaning. The exercises strengthen the foundation required for data science and data analytics workflows.


### Skills Practiced

Understanding Python data structures and logic
Working with lists and dictionaries
Using NumPy for numerical computations
Performing matrix operations
Handling datasets using Pandas
Cleaning missing data using statistical methods
Writing clean and structured code

### Submission

Completed independently and implemented structured Python solutions. Practiced real-world data handling concepts useful for data analysis.

Small data insights today lead to powerful decisions tomorrow.

#Python #NumPy #Pandas #DataScience #DataAnalytics #GitHub #DataAnalyst #LearningJourney #Coding #PythonProjects
