# CPP-OOPs
lab on C++ and oop concept
├── Program_01_Addition_Subtraction.cpp
├── Program_02_Swap_Using_Third_Variable.cpp
├── Program_03_Swap_Without_Third_Variable.cpp
├── Program_04_Area_Perimeter_Circle.cpp
├── Program_05_Celsius_To_Fahrenheit.cpp
"""
Assignment No. 2
Subject: Python Programming
Topic: Control Statements and Loops
"""

# -------------------------------------------------
# 1. Using if statement
# Write a Python program to add two numbers only if both numbers are positive.
# -------------------------------------------------

num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

if num1 > 0 and num2 > 0:
    print("Sum =", num1 + num2)


# -------------------------------------------------
# 2. Using if–else statement
# Write a Python program to find the maximum of two numbers using an if–else control structure.
# -------------------------------------------------

a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

if a > b:
    print("Maximum number is:", a)
else:
    print("Maximum number is:", b)


# -------------------------------------------------
# 3. Using for loop
# Write a Python program to compute the factorial of a given number using a for loop.
# -------------------------------------------------

num = int(input("Enter a number: "))
factorial = 1

for i in range(1, num + 1):
    factorial *= i

print("Factorial of", num, "is", factorial)


# -------------------------------------------------
# 4. Using if–elif–else statement
# Write a Python program to calculate Simple Interest, where different interest rates
# are applied using if–elif–else based on the time period.
# -------------------------------------------------

p = float(input("Enter principal amount: "))
t = int(input("Enter time period (in years): "))

if t <= 2:
    r = 5
elif t <= 5:
    r = 7
else:
    r = 10

si = (p * t * r) / 100
print("Simple Interest =", si)


# -------------------------------------------------
# 5. Using while loop and if condition
# Write a Python program to check whether a given number is an Armstrong number.
# -------------------------------------------------

number = int(input("Enter a number: "))
temp = number
sum = 0

while temp > 0:
    digit = temp % 10
    sum += digit ** 3
    temp //= 10

if sum == number:
    print(number, "is an Armstrong number")
else:
    print(number, "is not an Armstrong number")


# -------------------------------------------------
# 6. Using if condition
# Write a Python program to find the area of a circle only if the radius is greater than zero.
# -------------------------------------------------

radius = float(input("Enter radius: "))

if radius > 0:
    area = 3.14 * radius * radius
    print("Area of the circle =", area)


# -------------------------------------------------
# 7. Using for loop and range() function
# Write a Python program to print all prime numbers within a given interval.
# -------------------------------------------------

start = int(input("Enter starting number: "))
end = int(input("Enter ending number: "))

for num in range(start, end + 1):
    if num > 1:
        for i in range(2, num):
            if num % i == 0:
                break
        else:
            print(num)






# LAB on OOP Using C++ – Assignment 1

This repository contains C++ programs written for **Lab Assignment 1** of  
**Object Oriented Programming using C++**.

## Programs Included
1. Addition and Subtraction of two number#include <iostream>
using namespace std;

int main() {
    int a, b;
    cout << "Enter two numbers: ";
    cin >> a >> b;

    cout << "Addition = " << a + b << endl;
    cout << "Subtraction = " << a - b << endl;

    return 0;
}

2. Swap two numbers using third variable
   #include <iostream>
using namespace std;

int main() {
    int a, b, temp;
    cout << "Enter two numbers: ";
    cin >> a >> b;

    temp = a;
    a = b;
    b = temp;

    cout << "After swapping:" << endl;
    cout << "a = " << a << ", b = " << b << endl;

    return 0;
}

3. Swap two numbers without using third variable
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cout << "Enter two numbers: ";
    cin >> a >> b;

    a = a + b;
    b = a - b;
    a = a - b;

    cout << "After swapping:" << endl;
    cout << "a = " << a << ", b = " << b << endl;

    return 0;
}

4. Area and Perimeter of a Circle using constant
  #include <iostream>
using namespace std;

int main() {
    const float PI = 3.14;
    float radius;

    cout << "Enter radius: ";
    cin >> radius;

    cout << "Area of Circle = " << PI * radius * radius << endl;
    cout << "Perimeter of Circle = " << 2 * PI * radius << endl;

    return 0;
}

5. Celsius to Fahrenheit conversion
#include <iostream>
using namespace std;

int main() {
    float celsius, fahrenheit;

    cout << "Enter temperature in Celsius: ";
    cin >> celsius;

    fahrenheit = (celsius * 9 / 5) + 32;

    cout << "Temperature in Fahrenheit = " << fahrenheit << endl;

    return 0;
}

6. Check whether number is Positive, Negative or Zero
#include <iostream>
using namespace std;

int main() {
    int num;

    cout << "Enter a number: ";
    cin >> num;

    if (num > 0)
        cout << "Number is Positive";
    else if (num < 0)
        cout << "Number is Negative";
    else
        cout << "Number is Zero";

    return 0;
}


CPP-OOPs/
│
├── Program_01_Addition_Subtraction.cpp
├── Program_02_Swap_Using_Third_Variable.cpp
├── Program_03_Swap_Without_Third_Variable.cpp
├── Program_04_Area_Perimeter_Circle.cpp
├── Program_05_Celsius_To_Fahrenheit.cpp
└── Program_06_Positive_Negative_Zero.cpp


#include <iostream>
using namespace std;

int main() {
    int a, b, temp;
    cout << "Enter two numbers: ";
    cin >> a >> b;

    temp = a;
    a = b;
    b = temp;

    cout << "After swapping:" << endl;
    cout << "a = " << a << ", b = " << b << endl;

    return 0;
}

# CPP-OOPs

This repository contains C++ programs written for **Lab Assignment 1** of  
**Object Oriented Programming using C++**.

The focus is on building strong fundamentals using simple, clear programs.

---

## Lab Details
- **Subject:** Object Oriented Programming using C++
- **Assignment:** Lab Assignment 1
- **Language:** C++

---

## Repository Structure

Programs Included

Addition and Subtraction of Two Numbers
Takes two integers as input and displays their addition and subtraction.

Swap Two Numbers Using a Third Variable
Demonstrates swapping values using an extra temporary variable.

Swap Two Numbers Without Using a Third Variable
Performs swapping using arithmetic operations.

Area and Perimeter of a Circle
Calculates area and perimeter using a constant value of π.

Celsius to Fahrenheit Conversion
Converts temperature from Celsius to Fahrenheit using the standard formula.

Check Whether a Number is Positive, Negative, or Zero
Uses conditional statements to determine the nature of a number.

