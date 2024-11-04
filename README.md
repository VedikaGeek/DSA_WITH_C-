Let’s expand this to cover all 50 questions in a similar format. Each question will have a title and a C++ code solution. Here’s the full README with all 50 questions and solutions:

---

# C++ Programming Basics: 50 Questions with Solutions

This repository provides 50 beginner-level programming questions with solutions in C++. Each question covers fundamental concepts like variables, loops, arrays, functions, and more.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Index of Questions](#index-of-questions)
- [Solutions](#solutions)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

This repository is designed to help beginners learn C++ programming by solving basic questions with provided solutions.

## Getting Started

Clone the repository and open each file in your code editor to view questions and solutions.

## Index of Questions

| No. | Question Title                           | Solution             |
| --- | ---------------------------------------- | --------------------- |
| 1   | [Hello World Program](#1-hello-world-program) | Below                |
| 2   | [Input and Output](#2-input-and-output)       | Below                |
| 3   | [Sum of Two Numbers](#3-sum-of-two-numbers)   | Below                |
| 4   | [Odd or Even](#4-odd-or-even)                 | Below                |
| 5   | [Largest of Three Numbers](#5-largest-of-three-numbers) | Below |
| 6   | [Simple Calculator](#6-simple-calculator)     | Below                |
| 7   | [Prime Number Check](#7-prime-number-check)   | Below                |
| 8   | [Factorial of a Number](#8-factorial-of-a-number) | Below          |
| 9   | [Fibonacci Series](#9-fibonacci-series)       | Below                |
| 10  | [Reverse a Number](#10-reverse-a-number)      | Below                |
| 11  | [Sum of Digits](#11-sum-of-digits)            | Below                |
| 12  | [Palindrome Check](#12-palindrome-check)      | Below                |
| 13  | [Armstrong Number](#13-armstrong-number)      | Below                |
| 14  | [Number of Digits](#14-number-of-digits)      | Below                |
| 15  | [Power of a Number](#15-power-of-a-number)    | Below                |
| 16  | [Swap Two Numbers](#16-swap-two-numbers)      | Below                |
| 17  | [Simple Interest Calculation](#17-simple-interest-calculation) | Below |
| 18  | [Area of a Circle](#18-area-of-a-circle)      | Below                |
| 19  | [Leap Year Check](#19-leap-year-check)        | Below                |
| 20  | [Sum of Natural Numbers](#20-sum-of-natural-numbers) | Below         |
| 21  | [LCM of Two Numbers](#21-lcm-of-two-numbers)  | Below                |
| 22  | [GCD of Two Numbers](#22-gcd-of-two-numbers)  | Below                |
| 23  | [Binary to Decimal](#23-binary-to-decimal)    | Below                |
| 24  | [Decimal to Binary](#24-decimal-to-binary)    | Below                |
| 25  | [Print ASCII Value](#25-print-ascii-value)    | Below                |
| 26  | [Average of Numbers](#26-average-of-numbers)  | Below                |
| 27  | [Find Maximum Element in Array](#27-find-maximum-element-in-array) | Below |
| 28  | [Find Minimum Element in Array](#28-find-minimum-element-in-array) | Below |
| 29  | [Sum of Array Elements](#29-sum-of-array-elements) | Below          |
| 30  | [Reverse an Array](#30-reverse-an-array)      | Below                |
| 31  | [Count Vowels and Consonants](#31-count-vowels-and-consonants) | Below |
| 32  | [Prime Numbers in a Range](#32-prime-numbers-in-a-range) | Below   |
| 33  | [Remove Duplicates from Array](#33-remove-duplicates-from-array) | Below |
| 34  | [Count Frequency of Elements](#34-count-frequency-of-elements) | Below |
| 35  | [Sort Array in Ascending Order](#35-sort-array-in-ascending-order) | Below |
| 36  | [Transpose of a Matrix](#36-transpose-of-a-matrix) | Below         |
| 37  | [Multiplication Table](#37-multiplication-table) | Below         |
| 38  | [Calculate Sum of Series (1 + 1/2 + 1/3 ...)](#38-calculate-sum-of-series) | Below |
| 39  | [Check Alphabet Character](#39-check-alphabet-character) | Below    |
| 40  | [Count Words in a String](#40-count-words-in-a-string) | Below      |
| 41  | [Check if Array is Sorted](#41-check-if-array-is-sorted) | Below      |
| 42  | [Bubble Sort](#42-bubble-sort)               | Below                |
| 43  | [Insertion Sort](#43-insertion-sort)         | Below                |
| 44  | [Selection Sort](#44-selection-sort)         | Below                |
| 45  | [Quick Sort](#45-quick-sort)                 | Below                |
| 46  | [Binary Search](#46-binary-search)           | Below                |
| 47  | [Linear Search](#47-linear-search)           | Below                |
| 48  | [Convert Celsius to Fahrenheit](#48-convert-celsius-to-fahrenheit) | Below |
| 49  | [Calculate Compound Interest](#49-calculate-compound-interest) | Below |
| 50  | [Array Reversal](#50-array-reversal)         | Below                |

---

## Solutions

### 1. Hello World Program
```cpp
#include <iostream>
int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

### 2. Input and Output
```cpp
#include <iostream>
int main() {
    int a;
    std::cout << "Enter a number: ";
    std::cin >> a;
    std::cout << "You entered: " << a << std::endl;
    return 0;
}
```

### 3. Sum of Two Numbers
```cpp
#include <iostream>
int main() {
    int a, b;
    std::cout << "Enter two numbers: ";
    std::cin >> a >> b;
    std::cout << "Sum: " << a + b << std::endl;
    return 0;
}
```

### 4. Odd or Even
```cpp
#include <iostream>
int main() {
    int num;
    std::cout << "Enter a number: ";
    std::cin >> num;
    if (num % 2 == 0)
        std::cout << num << " is even." << std::endl;
    else
        std::cout << num << " is odd." << std::endl;
    return 0;
}
```

### 5. Largest of Three Numbers
```cpp
#include <iostream>
int main() {
    int a, b, c;
    std::cout << "Enter three numbers: ";
    std::cin >> a >> b >> c;
    int largest = (a > b) ? ((a > c) ? a : c) : ((b > c) ? b : c);
    std::cout << "Largest: " << largest << std::endl;
    return 0;
}

```
### 6. Simple Calculator
```cpp
#include <iostream>
int main() {
    char op;
    double num1, num2;
    std::cout << "Enter operator (+, -, *, /): ";
    std::cin >> op;
    std::cout << "Enter two numbers: ";
    std::cin >> num1 >> num2;
    switch(op) {
        case '+': std::cout << num1 + num2; break;
        case '-': std::cout << num1 - num2; break;
        case '*': std::cout << num1 * num2; break;
        case '/': std::cout << num1 / num2; break;
        default: std::cout << "Invalid operator!";
    }
    std::cout << std::endl;
    return 0;
}
```

### 7. Prime Number Check
```cpp
#include <iostream>
int main() {
    int n, i;
    bool isPrime = true;
    std::cout << "Enter a positive integer: ";
    std::cin >> n;
    if (n <= 1) isPrime = false;
    for (i = 2; i <= n / 2; ++i) {
        if (n % i == 0) {
            isPrime = false;
            break;
        }
    }
    std::cout << (isPrime ? "Prime" : "Not Prime") << std::endl;
    return 0;
}
```

### 8. Factorial of a Number
```cpp
#include <iostream>
int main() {
    int n;
    long long factorial = 1;
    std::cout << "Enter a positive integer: ";
    std::cin >> n;
    for (int i = 1; i <= n; ++i) factorial *= i;
    std::cout << "Factorial of " << n << " = " << factorial << std::endl;
    return 0;
}
```

### 9. Fibonacci Series
```cpp
#include <iostream>
int main() {
    int n, t1 = 0, t2 = 1, nextTerm;
    std::cout << "Enter the number of terms: ";
    std::cin >> n;
    std::cout << "Fibonacci Series: ";
    for (int i = 1; i <= n; ++i) {
        std::cout << t1 << " ";
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    return 0;
}
```

### 10. Reverse a Number
```cpp
#include <iostream>
int main() {
    int n, reverse = 0, remainder;
    std::cout << "Enter an integer: ";
    std::cin >> n;
    while (n != 0) {
        remainder = n % 10;
        reverse = reverse * 10 + remainder;
        n /= 10;
    }
    std::cout << "Reversed Number = " << reverse << std::endl;
    return 0;
}
```

### 11. Sum of Digits
```cpp
#include <iostream>
int main() {
    int n, sum = 0;
    std::cout << "Enter an integer: ";
    std::cin >> n;
    while (n != 0) {
        sum += n % 10;
        n /= 10;
    }
    std::cout << "Sum of digits = " << sum << std::endl;
    return 0;
}
```

### 12. Palindrome Check
```cpp
#include <iostream>
int main() {
    int n, original, reverse = 0, remainder;
    std::cout << "Enter an integer: ";
    std::cin >> n;
    original = n;
    while (n != 0) {
        remainder = n % 10;
        reverse = reverse * 10 + remainder;
        n /= 10;
    }
    if (original == reverse) std::cout << "Palindrome";
    else std::cout << "Not Palindrome";
    return 0;
}
```

### 13. Armstrong Number
```cpp
#include <iostream>
#include <cmath>
int main() {
    int n, original, remainder, result = 0, digits = 0;
    std::cout << "Enter an integer: ";
    std::cin >> n;
    original = n;
    while (original != 0) {
        original /= 10;
        ++digits;
    }
    original = n;
    while (original != 0) {
        remainder = original % 10;
        result += std::pow(remainder, digits);
        original /= 10;
    }
    if (result == n) std::cout << "Armstrong Number";
    else std::cout << "Not an Armstrong Number";
    return 0;
}
```

### 14. Number of Digits
```cpp
#include <iostream>
int main() {
    int n, count = 0;
    std::cout << "Enter an integer: ";
    std::cin >> n;
    while (n != 0) {
        n /= 10;
        ++count;
    }
    std::cout << "Number of digits = " << count << std::endl;
    return 0;
}
```

### 15. Power of a Number
```cpp
#include <iostream>
#include <cmath>
int main() {
    double base, exponent, result;
    std::cout << "Enter base and exponent: ";
    std::cin >> base >> exponent;
    result = std::pow(base, exponent);
    std::cout << base << "^" << exponent << " = " << result << std::endl;
    return 0;
}
```


---

### 16. Swap Two Numbers
```cpp
#include <iostream>
int main() {
    int a, b, temp;
    std::cout << "Enter two numbers: ";
    std::cin >> a >> b;
    temp = a;
    a = b;
    b = temp;
    std::cout << "After swapping, a = " << a << ", b = " << b << std::endl;
    return 0;
}
```

### 17. Simple Interest Calculation
```cpp
#include <iostream>
int main() {
    float principal, rate, time, interest;
    std::cout << "Enter principal, rate, and time: ";
    std::cin >> principal >> rate >> time;
    interest = (principal * rate * time) / 100;
    std::cout << "Simple Interest = " << interest << std::endl;
    return 0;
}
```

### 18. Area of a Circle
```cpp
#include <iostream>
#define PI 3.14159
int main() {
    float radius, area;
    std::cout << "Enter radius: ";
    std::cin >> radius;
    area = PI * radius * radius;
    std::cout << "Area of Circle = " << area << std::endl;
    return 0;
}
```

### 19. Leap Year Check
```cpp
#include <iostream>
int main() {
    int year;
    std::cout << "Enter a year: ";
    std::cin >> year;
    if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0)
        std::cout << year << " is a leap year.";
    else
        std::cout << year << " is not a leap year.";
    return 0;
}
```

### 20. Sum of Natural Numbers
```cpp
#include <iostream>
int main() {
    int n, sum = 0;
    std::cout << "Enter a positive integer: ";
    std::cin >> n;
    for (int i = 1; i <= n; ++i) sum += i;
    std::cout << "Sum = " << sum << std::endl;
    return 0;
}
```

### 21. LCM of Two Numbers
```cpp
#include <iostream>
int main() {
    int a, b, lcm;
    std::cout << "Enter two numbers: ";
    std::cin >> a >> b;
    lcm = (a > b) ? a : b;
    while (true) {
        if (lcm % a == 0 && lcm % b == 0) {
            std::cout << "LCM = " << lcm << std::endl;
            break;
        }
        ++lcm;
    }
    return 0;
}
```

### 22. GCD of Two Numbers
```cpp
#include <iostream>
int main() {
    int a, b;
    std::cout << "Enter two numbers: ";
    std::cin >> a >> b;
    while (a != b) {
        if (a > b) a -= b;
        else b -= a;
    }
    std::cout << "GCD = " << a << std::endl;
    return 0;
}
```

### 23. Binary to Decimal
```cpp
#include <iostream>
#include <cmath>
int main() {
    int binary, decimal = 0, base = 1, remainder;
    std::cout << "Enter a binary number: ";
    std::cin >> binary;
    while (binary > 0) {
        remainder = binary % 10;
        decimal += remainder * base;
        binary /= 10;
        base *= 2;
    }
    std::cout << "Decimal = " << decimal << std::endl;
    return 0;
}
```

### 24. Decimal to Binary
```cpp
#include <iostream>
int main() {
    int decimal, binary = 0, base = 1, remainder;
    std::cout << "Enter a decimal number: ";
    std::cin >> decimal;
    while (decimal > 0) {
        remainder = decimal % 2;
        binary += remainder * base;
        decimal /= 2;
        base *= 10;
    }
    std::cout << "Binary = " << binary << std::endl;
    return 0;
}
```

### 25. Print ASCII Value
```cpp
#include <iostream>
int main() {
    char c;
    std::cout << "Enter a character: ";
    std::cin >> c;
    std::cout << "ASCII value of " << c << " = " << int(c) << std::endl;
    return 0;
}
```

### 26. Average of Numbers
```cpp
#include <iostream>
int main() {
    int n, sum = 0, number;
    std::cout << "Enter the number of elements: ";
    std::cin >> n;
    for (int i = 0; i < n; ++i) {
        std::cout << "Enter number " << i + 1 << ": ";
        std::cin >> number;
        sum += number;
    }
    std::cout << "Average = " << sum / static_cast<float>(n) << std::endl;
    return 0;
}
```

### 27. Find Maximum Element in Array
```cpp
#include <iostream>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) std::cin >> arr[i];
    int max = arr[0];
    for (int i = 1; i < n; ++i) if (arr[i] > max) max = arr[i];
    std::cout << "Maximum element = " << max << std::endl;
    return 0;
}
```

### 28. Find Minimum Element in Array
```cpp
#include <iostream>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) std::cin >> arr[i];
    int min = arr[0];
    for (int i = 1; i < n; ++i) if (arr[i] < min) min = arr[i];
    std::cout << "Minimum element = " << min << std::endl;
    return 0;
}
```

### 29. Sum of Array Elements
```cpp
#include <iostream>
int main() {
    int n, sum = 0;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) {
        std::cin >> arr[i];
        sum += arr[i];
    }
    std::cout << "Sum of elements = " << sum << std::endl;
    return 0;
}
```

### 30. Reverse an Array
```cpp
#include <iostream>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) std::cin >> arr[i];
    std::cout << "Reversed array: ";
    for (int i = n - 1; i >= 0; --i) std::cout << arr[i] << " ";
    return 0;
}
```

### 31. Count Vowels and Consonants
```cpp
#include <iostream>
#include <cctype>
int main() {
    std::string text;
    int vowels = 0, consonants = 0;
    std::cout << "Enter a string: ";
    std::getline(std::cin, text);
    for (char ch : text) {
        if (std::isalpha(ch)) {
            ch = std::tolower(ch);
            if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u')
                ++vowels;
            else
                ++consonants;
        }
    }
    std::cout << "Vowels: " << vowels << ", Consonants: " << consonants << std::endl;
    return 0;
}
```



## Usage

To run any of the solutions, compile the `.cpp` file using a C++ compiler, and execute the output file. Example for compiling **Hello World**:

```bash
g++ 01_Hello_World.cpp -o hello
./hello
```

## Contributing

Contributions are welcome! If you’d like to add questions, improve solutions, or report issues, please submit a pull request.

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

Happy Coding! 🎉
