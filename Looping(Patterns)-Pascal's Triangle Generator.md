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
~~~c
def generate_pascals_triangle(rows):
    triangle = []
    for i in range(rows):
        row = [1]
        if triangle:
            last_row = triangle[-1]
            row.extend([last_row[j] + last_row[j + 1] for j in range(len(last_row) - 1)])
            row.append(1)
        triangle.append(row)
    return triangle
num_rows = int(input("Enter the number of rows: "))
pascals_triangle = generate_pascals_triangle(num_rows)
for row in pascals_triangle:
    print(" ".join(map(str, row)).center(num_rows * 2))
~~~

## Sample Output

![Screenshot 2025-05-11 093916](https://github.com/user-attachments/assets/fedc7da9-4b40-4659-ab14-47e079a19bd4)


## Result

Thus,the program has been executed successfully.

