Data Science (Task Day-02)

## Phase: Python

## Focus Area: Variables

---

## Problem Statement

Write a Python program to accept employee salary data and calculate annual salary and tax deduction.

---

## Description

This program takes employee details such as name, monthly salary, and tax rate, then calculates:

* Annual Salary
* Tax Deducted
* Take Home Salary

This demonstrates the use of Python variables, user input, and arithmetic operations in a real-world scenario.

---

## Skills Practiced

* Variables and Data Types
* User Input Handling
* Arithmetic Calculations
* Logical Thinking
* Clean Code Structure

---

## Python Code

```python
name = input("Enter your name: ")
monthly_salary = float(input("Enter your monthly salary: "))
tax_rate = float(input("Enter tax rate in percent: "))

annual_salary = monthly_salary * 12
tax_amount = (tax_rate / 100) * annual_salary
take_home = annual_salary - tax_amount

print("Salary Report for", name)
print("Monthly Salary  :", monthly_salary)
print("Annual Salary   :", annual_salary)
print("Tax Rate        :", tax_rate, "%")
print("Tax Deducted    :", tax_amount)
print("Take Home Salary:", take_home)
```

---

## Sample Output

```
Enter your name: Shivansh
Enter your monthly salary: 50000
Enter tax rate in percent: 10

Salary Report for Shivansh
Monthly Salary  : 50000.0
Annual Salary   : 600000.0
Tax Rate        : 10.0 %
Tax Deducted    : 60000.0
Take Home Salary: 540000.0
```

---

## Learning Outcome

* Learned how to take user input in Python
* Used variables for calculations
* Applied tax percentage logic
* Wrote structured and readable code

---

Small calculations today build the foundation for big data decisions tomorrow.
