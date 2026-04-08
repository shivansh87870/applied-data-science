Python Data Science Practice — ABTalks Season 3
Task Day 04, Day 05, Day 06

Task Day 04
Phase: Python
Focus Area: Loops
Problem Statement: Given daily sales data for a week, calculate total and average sales using loops.

Solution:

```python
sales = [1200, 1500, 1100, 1800, 2000, 1700, 1600]

total_sales = 0
for s in sales:
    total_sales += s

average_sales = total_sales / len(sales)

print("Total Sales:", total_sales)
print("Average Sales:", average_sales)
```

Output:

```
Total Sales: 10900
Average Sales: 1557.142857142857
```

Task Day 05
Phase: Python
Focus Area: Functions
Problem Statement: Create Python functions to calculate mean, median, and mode for a list of numbers.

Solution:

```python
def mean(data):
    return sum(data) / len(data)

def median(data):
    data = sorted(data)
    n = len(data)
    mid = n // 2
    if n % 2 == 0:
        return (data[mid-1] + data[mid]) / 2
    else:
        return data[mid]

def mode(data):
    freq = {}
    for num in data:
        freq[num] = freq.get(num, 0) + 1
    max_freq = max(freq.values())
    return [k for k, v in freq.items() if v == max_freq]

numbers = [1, 2, 2, 3, 4, 5, 2, 6]

print("Mean:", mean(numbers))
print("Median:", median(numbers))
print("Mode:", mode(numbers))
```

Output:

```
Mean: 3.125
Median: 2.5
Mode: [2]
```

Task Day 06
Phase: Python
Focus Area: Data Structures
Problem Statement: Count frequency of words in a sentence using dictionary.

Solution:

```python
sentence = "data science is fun and data science is powerful"
words = sentence.split()

frequency = {}

for word in words:
    frequency[word] = frequency.get(word, 0) + 1

print(frequency)
```

Output:

```
{'data': 2, 'science': 2, 'is': 2, 'fun': 1, 'and': 1, 'powerful': 1}
```

Challenge Overview
These tasks focus on applying Python fundamentals to real-world data scenarios including aggregation, statistical computation, and text analysis. The exercises strengthen the foundation required for data science and data analytics workflows.

Skills Practiced
Understanding loop constructs in Python
Writing reusable Python functions
Working with lists and numerical data
Calculating statistical measures
Using dictionaries for data mapping
Performing aggregation and analysis
Writing clean and structured code

Submission
Completed independently and implemented structured Python solutions. Practiced real-world data handling concepts useful for data analysis.

Small data insights today lead to powerful decisions tomorrow.

#Python #DataScience #DataAnalytics #GitHub #DataAnalyst #LearningJourney #Coding #PythonProjects
