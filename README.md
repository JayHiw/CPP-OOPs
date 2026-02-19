# OOPs using CPP
lab on C++ and oop concept
├── Program_01_Addition_Subtraction.cpp
├── Program_02_Swap_Using_Third_Variable.cpp
├── Program_03_Swap_Without_Third_Variable.cpp
├── Program_04_Area_Perimeter_Circle.cpp
├── Program_05_Celsius_To_Fahrenheit.cpp
 Assignment No. 2
# 1. Using if statement
# Write a Python program to add two numbers only if both numbers are positive.


num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

if num1 > 0 and num2 > 0:



# 2. Using if–else statement
# Write a Python program to find the maximum of two numbers using an if–else control structure.
# -------------------------------------------------

a = float(input("Enter first number: "))
b = float(input("Enter second number: "))

if a > b:
    print("Maximum number is:", a)
else:
    print("Maximum number is:", b)


# 3. Using for loop
# Write a Python program to compute the factorial of a given number using a for loop.


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


assignment 04
LAB on OOP Using CPP

Assigment-4

1)	Write a CPP program to display Fibonacci series using recursion.
2)	Write a CPP program to find perimeter of a circle using inline function.
3)	Write a menu driven CPP program for following options. 
i.	To find square root of a number 
ii.	To find ceil value of a number
iii.	To find rounded value of a number
iv.	To evaluate a^b operation 
4)	Write a menu driven CPP program for following options using function overloading concept.
i.	To calculate area of square 
ii.	To calculate area of rectangle
iii.	To calculate area of circle
5)	Write a menu driven CPP program for following options using function overloading concept
i.	To find a raised to b
ii.	To find summation of first n integers
iii.	To find multiplication of two numbers


solutions :- 

#include <iostream>
using namespace std;

int fibonacci(int n) {
    if (n == 0)
        return 0;
    else if (n == 1)
        return 1;
    else
        return fibonacci(n - 1) + fibonacci(n - 2);
}

int main() {
    int n;
    cout << "Enter number of terms: ";
    cin >> n;

    cout << "Fibonacci Series: ";
    for (int i = 0; i < n; i++) {
        cout << fibonacci(i) << " ";
    }

    return 0;
}



4) Menu Driven Program using Function Overloading (Area)
#include <iostream>
using namespace std;

float area(float side) {
    return side * side;
}

float area(float length, float breadth) {
    return length * breadth;
}

float area(double radius) {
    return 3.14 * radius * radius;
}

int main() {
    int choice;
    float a, b;
    double r;

    cout << "1. Area of Square\n";
    cout << "2. Area of Rectangle\n";
    cout << "3. Area of Circle\n";
    cout << "Enter choice: ";
    cin >> choice;

    switch (choice) {
        case 1:
            cout << "Enter side: ";
            cin >> a;
            cout << "Area of Square: " << area(a);
            break;

        case 2:
            cout << "Enter length and breadth: ";
            cin >> a >> b;
            cout << "Area of Rectangle: " << area(a, b);
            break;

        case 3:
            cout << "Enter radius: ";
            cin >> r;
            cout << "Area of Circle: " << area(r);
            break;

        default:
            cout << "Invalid Choice";
    }

    return 0;
}

3) Perimeter of a Circle using Inline Function
#include <iostream>
using namespace std;

inline float perimeter(float r) {
    return 2 * 3.14 * r;
}

int main() {
    float radius;
    cout << "Enter radius: ";
    cin >> radius;

    cout << "Perimeter of circle: " << perimeter(radius);

    return 0;
}



3) Menu Driven Program (Math Functions)
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    int choice;
    double num, a, b;

    cout << "1. Square Root\n";
    cout << "2. Ceil Value\n";
    cout << "3. Rounded Value\n";
    cout << "4. Power (a^b)\n";
    cout << "Enter your choice: ";
    cin >> choice;

    switch (choice) {
        case 1:
            cout << "Enter number: ";
            cin >> num;
            cout << "Square Root: " << sqrt(num);
            break;

        case 2:
            cout << "Enter number: ";
            cin >> num;
            cout << "Ceil Value: " << ceil(num);
            break;

        case 3:
            cout << "Enter number: ";
            cin >> num;
            cout << "Rounded Value: " << round(num);
            break;

        case 4:
            cout << "Enter a and b: ";
            cin >> a >> b;
            cout << "Result: " << pow(a, b);
            break;

        default:
            cout << "Invalid Choice";
    }

    return 0;
}



