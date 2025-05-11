# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
~~~c
def compute_modulo(a, b):
    return a % b
num1 = int(input("Enter a number: "))
num2 = int(input("Enter a number: "))
result = compute_modulo(num1, num2)
print(f"The modulo of {num1} % {num2} is {result}")
~~~

## Output

![Screenshot 2025-05-11 093133 - Copy](https://github.com/user-attachments/assets/7bceb262-7651-4217-8cc3-60ae18186676)


## Result
Thus , the program has been executed succesfully.
