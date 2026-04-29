c-programes
# Circle Area & Perimeter Program in C

This is a simple C program that calculates:

- Area of a Circle
- Perimeter (Circumference) of a Circle

## Formula Used

Area = π × r × r  
Perimeter = 2 × π × r  

## Concepts Used

- Macros (#define)
- User Input using scanf
- Floating point calculations
- Basic mathematical operations

## Author

Basavaraj S  
Electronics & Communication Engineering Student

## 🔷 Program: Largest Value in an Array

### 📌 Description
This program finds the **largest number in a float array** using a function.

---

### 💻 Program
```c
#include <stdio.h>

float largest(float a[], int n);

main()
{
    float largest(float a[], int n);
    float value[4] = {2.65, 4.75, 1.2, 3.66};

    printf("%f\n", largest(value, 4));
}

float largest(float a[], int n)
{
    int i;
    float max;

    max = a[0];

    for(i = 1; i < n; i++)
    {
        if(max < a[i])
            max = a[i];
    }

    return max;
}
```

---

### 📊 Sample Output
```
4.750000
```

---

### 🧠 Concepts Used
- Functions
- Arrays
- Loop (for loop)
- Conditional statements (if)
- Floating point numbers