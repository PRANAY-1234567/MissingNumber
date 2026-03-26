📘 Python Program: Find Missing Number in a List

📌 Overview

This Python program finds the missing number from a sequence of numbers.
It assumes that the list contains numbers from 1 to n, with one number missing.

⚙️ Source Code
arr = [1, 2, 3, 5]
n = 5

total = n * (n + 1) // 2
sum_arr = sum(arr)

missing = total - sum_arr

print("Missing number is:", missing)

🧠 How It Works
1️⃣ Understand the Problem

Given:

arr = [1, 2, 3, 5]

Expected sequence:

1, 2, 3, 4, 5

👉 Missing number is 4

2️⃣ Calculate Expected Sum
total = n * (n + 1) // 2

Formula for sum of first n natural numbers:

𝑛
(
𝑛
+
1
)
/
2
n(n+1)/2

Example:

5 * 6 / 2 = 15
3️⃣ Calculate Actual Sum
sum_arr = sum(arr)
Adds all elements in the list

Example:

1 + 2 + 3 + 5 = 11
4️⃣ Find Missing Number
missing = total - sum_arr
15 - 11 = 4
5️⃣ Print Result
print("Missing number is:", missing)
▶️ Output
Missing number is: 4
🔑 Key Concepts Used
Mathematical formula (sum of n numbers)
Lists
Built-in function sum()
Arithmetic operations
⏱️ Time Complexity
O(n) → for calculating sum of the list
⚠️ Important Assumptions
Numbers are from 1 to n
Only one number is missing
No duplicate values
🚀 Alternative Approach (Using Loop)
missing = 0
for i in range(1, n+1):
    if i not in arr:
        missing = i
        break

print("Missing number is:", missing)
📚 Learning Outcome

After understanding this program, you will learn:

How to solve problems using mathematical formulas
How to work with lists in Python
How to optimize solutions instead of using loops
