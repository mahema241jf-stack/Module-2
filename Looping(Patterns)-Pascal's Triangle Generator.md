# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
import math

rows = int(input("Enter the number of rows: "))

for n in range(rows):
    for space in range(rows - n - 1):
        print(" ", end="")

    for k in range(n + 1):
        value = math.factorial(n) // (math.factorial(k) * math.factorial(n - k))
        print(value, end=" ")

    print()
```

## Sample Output
<img width="427" height="289" alt="{96CAADEB-8E8A-4A35-9537-F5BF1293BCEF}" src="https://github.com/user-attachments/assets/c8463176-58ea-49bd-b018-d76a477018df" />

## Result
The program successfully generates and displays Pascal’s Triangle for the number of rows entered by the user using the combination formula.
