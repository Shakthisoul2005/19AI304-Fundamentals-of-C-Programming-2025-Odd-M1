# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int intLiteral = 111;
    float floatLiteral = 1.11;
    char charLiteral = 'D';
    char stringLiteral[] = "Hello C";

    printf("Integer literal: %d, Size: %lu bytes\n", intLiteral, sizeof(intLiteral));
    printf("Float literal: %f, Size: %lu bytes\n", floatLiteral, sizeof(floatLiteral));
    printf("Character literal: %c, Size: %lu bytes\n", charLiteral, sizeof(charLiteral));
    printf("String literal: %s, Size: %lu bytes\n", stringLiteral, sizeof(stringLiteral));

    return 0;
}
```

# Output:
<img width="459" height="265" alt="Screenshot 2025-11-18 211531" src="https://github.com/user-attachments/assets/2da8f420-2351-49f2-bec7-b2d5d60879af" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>

#define PI 3.14159    // Macro constant

int main() {
    const int AGE = 21;   // Constant variable

    printf("Value of macro constant PI: %f\n", PI);
    printf("Value of constant variable AGE: %d\n", AGE);

    return 0;
}
```
# Output:
<img width="406" height="131" alt="Screenshot 2025-11-18 211948" src="https://github.com/user-attachments/assets/fdfadb45-c8da-4e11-b7b5-d7b76825da1c" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>
int main() {
    int num = 25;             
    float rate = 12.5f;       
    double amount = 12345.6789; 
    char grade = 'A';         

    printf("Integer value (int): %d\n", num);
    printf("Float value (float): %f\n", rate);
    printf("Double value (double): %lf\n", amount);
    printf("Character value (char): %c\n", grade);

    return 0;
}
```
# Output:
<img width="390" height="193" alt="Screenshot 2025-11-18 212140" src="https://github.com/user-attachments/assets/d4c46779-7b1a-47e9-b51c-05be7071e99a" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
    int a, b;
    scanf("%d %d", &a, &b);

    printf("Addition: %d\n", a + b);
    printf("Subtraction: %d\n", a - b);
    printf("Multiplication: %d\n", a * b);

    if (b != 0)
        printf("Division: %d\n", a / b);
    else
        printf("Division: undefined\n");

    if (b != 0)
        printf("Remainder: %d\n", a % b);
    else
        printf("Remainder: undefined\n");

    printf("Bitwise AND: %d\n", a & b);
    printf("Bitwise OR: %d\n", a | b);
    printf("Bitwise XOR: %d\n", a ^ b);
    printf("Left Shift (a<<1): %d\n", a << 1);
    printf("Right Shift (a>>1): %d\n", a >> 1);
    printf("NOT of a: %d\n", ~a);

    return 0;
}
```
# Output:
<img width="260" height="353" alt="Screenshot 2025-11-18 212414" src="https://github.com/user-attachments/assets/88517651-a724-4e74-86d4-974353d13008" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char ch = '#';

    (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U') ?
        printf("Vowel") :
    (isalpha(ch) ? printf("Consonant") :
    (isdigit(ch) ? printf("Digit") : printf("Special Symbol")));

    return 0;
}
```
# Output:
<img width="380" height="195" alt="Screenshot 2025-11-18 212615" src="https://github.com/user-attachments/assets/e9f0d805-0ccb-4e5d-8405-e4c234696036" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


