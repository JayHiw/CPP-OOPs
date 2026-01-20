# CPP-OOPs
lab on C++ and oop concept
├── Program_01_Addition_Subtraction.cpp
├── Program_02_Swap_Using_Third_Variable.cpp
├── Program_03_Swap_Without_Third_Variable.cpp
├── Program_04_Area_Perimeter_Circle.cpp
├── Program_05_Celsius_To_Fahrenheit.cpp
└── Program_06_Positive_Negative_Zero.cpp





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



