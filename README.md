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

functiones 04 
## 🔷 Program: Sorting an Array Using Function (Bubble Sort)

### 📌 Description
This program sorts an array of integers in **ascending order** using a function.  
It uses the **Bubble Sort algorithm** to compare and swap adjacent elements.

---

### 💻 Program
```c
#include <stdio.h>

void sort(int n, int x[]);

main()
{
    int i;
    int marks[5] = {40, 90, 73, 81, 85};

    printf("marks before sorting\n");
    for(i = 0; i < 5; i++)
        printf("%d ", marks[i]);

    printf("\n\n");

    sort(5, marks);   // function call

    printf("marks after sorting\n");
    for(i = 0; i < 5; i++)
        printf("%4d", marks[i]);

    printf("\n");
}

void sort(int n, int x[])
{
    int i, j, t;

    for(i = 1; i <= n - 1; i++)
    {
        for(j = 1; j <= n - i; j++)
        {
            if(x[j - 1] > x[j])
            {
                t = x[j - 1];
                x[j - 1] = x[j];
                x[j] = t;
            }
        }
    }
}
```

---

### 📊 Sample Output
```
marks before sorting
40 90 73 81 85

marks after sorting
  40  73  81  85  90
```

---

### 🧠 Concepts Used
- Functions
- Arrays
- Bubble Sort Algorithm
- Nested loops
- Conditional statements (if)
- Swapping technique

---

### ⚙️ Algorithm (Steps)
1. Start from the first element of the array  
2. Compare adjacent elements  
3. Swap if they are in wrong order  
4. Repeat for all elements  
5. Continue passes until array is sorted  

---

### 👨‍💻 Author
Basavaraj S  
Electronics & Communication Engineering Student

5) Function-5
Even or Odd Using Function in C

📌 Description

This program checks whether a given number is even or odd using a function in C.

---

🧠 Concept Used

- Functions in C
- Modulus operator ("%")
- Conditional statements ("if-else")

---

⚙️ How It Works

1. User enters a number.
2. The number is passed to a function.
3. The function uses:
   n % 2
   - If result = "0" → Even
   - If result = "1" → Odd
4. The result is returned to "main()" and printed.

---

💻 Code

#include <stdio.h>

// function declaration
int checkEvenOdd(int n);

int main()
{
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (checkEvenOdd(num) == 0)
        printf("Even number");
    else
        printf("Odd number");

    return 0;
}

// function definition
int checkEvenOdd(int n)
{
    return n % 2;
}

---

▶️ Sample Input / Output

Input:

Enter a number: 6

Output:

Even number

Input:

Enter a number: 5

Output:

Odd number

---

📚 Key Learning

- "%" operator gives remainder
- Functions help in code reuse
- Clear separation of logic (main vs function)

---

🚀 Future Improvements

- Take multiple numbers as input
- Print result inside function
- Extend for positive/negative checks

---