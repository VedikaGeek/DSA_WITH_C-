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

Sure! Here's the clickable index for the README, formatted for easy navigation:

---



## Index

1. [Hello World Program](#1-hello-world-program)
2. [Sum of Two Numbers](#2-sum-of-two-numbers)
3. [Difference of Two Numbers](#difference-of-two-numbers)
4. [Multiplication of Two Numbers](#multiplication-of-two-numbers)
5. [Division of Two Numbers](#division-of-two-numbers)
6. [Check Even or Odd](#check-even-or-odd)
7. [Find Largest of Three Numbers](#find-largest-of-three-numbers)
8. [Check Prime Number](#check-prime-number)
9. [Check Armstrong Number](#check-armstrong-number)
10. [Reverse a Number](#reverse-a-number)
11. [Sum of Digits of a Number](#sum-of-digits-of-a-number)
12. [Count Digits in a Number](#count-digits-in-a-number)
13. [Fibonacci Series](#fibonacci-series)
14. [Factorial of a Number](#factorial-of-a-number)
15. [Temperature Conversion (Celsius to Fahrenheit)](#temperature-conversion-celsius-to-fahrenheit)
16. [Swap Two Numbers](#swap-two-numbers)
17. [Simple Interest Calculation](#simple-interest-calculation)
18. [Area of a Circle](#area-of-a-circle)
19. [Leap Year Check](#leap-year-check)
20. [Sum of Natural Numbers](#sum-of-natural-numbers)
21. [LCM of Two Numbers](#lcm-of-two-numbers)
22. [GCD of Two Numbers](#gcd-of-two-numbers)
23. [Binary to Decimal Conversion](#binary-to-decimal-conversion)
24. [Decimal to Binary Conversion](#decimal-to-binary-conversion)
25. [Print ASCII Value](#print-ascii-value)
26. [Average of Numbers](#average-of-numbers)
27. [Find Maximum Element in Array](#find-maximum-element-in-array)
28. [Find Minimum Element in Array](#find-minimum-element-in-array)
29. [Sum of Array Elements](#sum-of-array-elements)
30. [Reverse an Array](#reverse-an-array)
31. [Count Vowels and Consonants](#count-vowels-and-consonants)
32. [Check if a String is a Palindrome](#check-if-a-string-is-a-palindrome)
33. [Find Factorial Using Recursion](#find-factorial-using-recursion)
34. [Find Fibonacci Series Using Recursion](#find-fibonacci-series-using-recursion)
35. [Convert Celsius to Fahrenheit](#convert-celsius-to-fahrenheit)
36. [Find Largest and Smallest Number in Array](#find-largest-and-smallest-number-in-array)
37. [Transpose of a Matrix](#transpose-of-a-matrix)
38. [Sum of Each Row and Column in a Matrix](#sum-of-each-row-and-column-in-a-matrix)
39. [Count Frequency of Elements in an Array](#count-frequency-of-elements-in-an-array)
40. [Sort Array in Ascending Order](#sort-array-in-ascending-order)
41. [Find Median of Array](#find-median-of-array)
42. [Find Mode of Array](#find-mode-of-array)
43. [Reverse a String](#reverse-a-string)
44. [Find Length of a String](#find-length-of-a-string)
45. [Convert String to Uppercase](#convert-string-to-uppercase)
46. [Convert String to Lowercase](#convert-string-to-lowercase)
47. [Remove Vowels from a String](#remove-vowels-from-a-string)
48. [Count Words in a Sentence](#count-words-in-a-sentence)
49. [Find Sum of Digits in an Integer](#find-sum-of-digits-in-an-integer)
50. [Reverse a Number](#reverse-a-number)

---

Feel free to let me know if you need anything else!
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



---

### 32. Check if a String is a Palindrome
```cpp
#include <iostream>
#include <algorithm>
int main() {
    std::string str, rev;
    std::cout << "Enter a string: ";
    std::cin >> str;
    rev = str;
    std::reverse(rev.begin(), rev.end());
    if (str == rev)
        std::cout << "The string is a palindrome." << std::endl;
    else
        std::cout << "The string is not a palindrome." << std::endl;
    return 0;
}
```

### 33. Find Factorial Using Recursion
```cpp
#include <iostream>
int factorial(int n) {
    if (n <= 1) return 1;
    return n * factorial(n - 1);
}
int main() {
    int n;
    std::cout << "Enter a positive integer: ";
    std::cin >> n;
    std::cout << "Factorial of " << n << " = " << factorial(n) << std::endl;
    return 0;
}
```

### 34. Find Fibonacci Series Using Recursion
```cpp
#include <iostream>
int fibonacci(int n) {
    if (n <= 1) return n;
    return fibonacci(n - 1) + fibonacci(n - 2);
}
int main() {
    int n;
    std::cout << "Enter the number of terms: ";
    std::cin >> n;
    std::cout << "Fibonacci Series: ";
    for (int i = 0; i < n; i++) std::cout << fibonacci(i) << " ";
    return 0;
}
```

### 35. Convert Celsius to Fahrenheit
```cpp
#include <iostream>
int main() {
    float celsius, fahrenheit;
    std::cout << "Enter temperature in Celsius: ";
    std::cin >> celsius;
    fahrenheit = (celsius * 9/5) + 32;
    std::cout << "Temperature in Fahrenheit: " << fahrenheit << std::endl;
    return 0;
}
```

### 36. Find Largest and Smallest Number in Array
```cpp
#include <iostream>
#include <climits>
int main() {
    int n, largest = INT_MIN, smallest = INT_MAX;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) {
        std::cin >> arr[i];
        if (arr[i] > largest) largest = arr[i];
        if (arr[i] < smallest) smallest = arr[i];
    }
    std::cout << "Largest = " << largest << ", Smallest = " << smallest << std::endl;
    return 0;
}
```

### 37. Transpose of a Matrix
```cpp
#include <iostream>
int main() {
    int rows, cols;
    std::cout << "Enter rows and columns of matrix: ";
    std::cin >> rows >> cols;
    int matrix[rows][cols], transpose[cols][rows];
    std::cout << "Enter matrix elements:\n";
    for (int i = 0; i < rows; ++i)
        for (int j = 0; j < cols; ++j) std::cin >> matrix[i][j];
    for (int i = 0; i < rows; ++i)
        for (int j = 0; j < cols; ++j) transpose[j][i] = matrix[i][j];
    std::cout << "Transpose of matrix:\n";
    for (int i = 0; i < cols; ++i) {
        for (int j = 0; j < rows; ++j) std::cout << transpose[i][j] << " ";
        std::cout << std::endl;
    }
    return 0;
}
```

### 38. Sum of Each Row and Column in a Matrix
```cpp
#include <iostream>
int main() {
    int rows, cols;
    std::cout << "Enter rows and columns: ";
    std::cin >> rows >> cols;
    int matrix[rows][cols];
    std::cout << "Enter matrix elements:\n";
    for (int i = 0; i < rows; ++i)
        for (int j = 0; j < cols; ++j) std::cin >> matrix[i][j];
    std::cout << "Row sums: ";
    for (int i = 0; i < rows; ++i) {
        int rowSum = 0;
        for (int j = 0; j < cols; ++j) rowSum += matrix[i][j];
        std::cout << rowSum << " ";
    }
    std::cout << "\nColumn sums: ";
    for (int j = 0; j < cols; ++j) {
        int colSum = 0;
        for (int i = 0; i < rows; ++i) colSum += matrix[i][j];
        std::cout << colSum << " ";
    }
    return 0;
}
```

### 39. Count Frequency of Elements in an Array
```cpp
#include <iostream>
#include <map>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::map<int, int> frequency;
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) {
        std::cin >> arr[i];
        ++frequency[arr[i]];
    }
    std::cout << "Element frequencies:\n";
    for (auto &elem : frequency) std::cout << elem.first << ": " << elem.second << "\n";
    return 0;
}
```

### 40. Sort Array in Ascending Order
```cpp
#include <iostream>
#include <algorithm>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) std::cin >> arr[i];
    std::sort(arr, arr + n);
    std::cout << "Sorted array: ";
    for (int i = 0; i < n; ++i) std::cout << arr[i] << " ";
    return 0;
}
```

### 41. Find Median of Array
```cpp
#include <iostream>
#include <algorithm>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) std::cin >> arr[i];
    std::sort(arr, arr + n);
    double median;
    if (n % 2 == 0)
        median = (arr[n / 2 - 1] + arr[n / 2]) / 2.0;
    else
        median = arr[n / 2];
    std::cout << "Median = " << median << std::endl;
    return 0;
}
```

### 42. Find Mode of Array
```cpp
#include <iostream>
#include <map>
#include <vector>
int main() {
    int n;
    std::cout << "Enter number of elements: ";
    std::cin >> n;
    int arr[n];
    std::map<int, int> frequency;
    std::cout << "Enter elements: ";
    for (int i = 0; i < n; ++i) {
        std::cin >> arr[i];
        ++frequency[arr[i]];
    }
    int mode = arr[0], maxCount = 0;
    for (auto &elem : frequency) {
        if (elem.second > maxCount) {
            mode = elem.first;
            maxCount = elem.second;
        }
    }
    std::cout << "Mode = " << mode << std::endl;
    return 0;
}
```

### 43. Reverse a String
```cpp
#include <iostream>
#include <algorithm>
int main() {
    std::string str;
    std::cout << "Enter a string: ";
    std::cin >> str;
    std::reverse(str.begin(), str.end());
    std::cout << "Reversed string: " << str << std::endl;
    return 0;
}
```



---

### 44. Find Length of a String
```cpp
#include <iostream>
int main() {
    std::string str;
    std::cout << "Enter a string: ";
    std::cin >> str;
    std::cout << "Length of the string = " << str.length() << std::endl;
    return 0;
}
```

### 45. Convert String to Uppercase
```cpp
#include <iostream>
#include <algorithm>
int main() {
    std::string str;
    std::cout << "Enter a string: ";
    std::cin >> str;
    std::transform(str.begin(), str.end(), str.begin(), ::toupper);
    std::cout << "Uppercase string: " << str << std::endl;
    return 0;
}
```

### 46. Convert String to Lowercase
```cpp
#include <iostream>
#include <algorithm>
int main() {
    std::string str;
    std::cout << "Enter a string: ";
    std::cin >> str;
    std::transform(str.begin(), str.end(), str.begin(), ::tolower);
    std::cout << "Lowercase string: " << str << std::endl;
    return 0;
}
```

### 47. Remove Vowels from a String
```cpp
#include <iostream>
int main() {
    std::string str, result;
    std::cout << "Enter a string: ";
    std::cin >> str;
    for (char ch : str) {
        if (ch != 'a' && ch != 'e' && ch != 'i' && ch != 'o' && ch != 'u' &&
            ch != 'A' && ch != 'E' && ch != 'I' && ch != 'O' && ch != 'U') {
            result += ch;
        }
    }
    std::cout << "String without vowels: " << result << std::endl;
    return 0;
}
```

### 48. Count Words in a Sentence
```cpp
#include <iostream>
#include <sstream>
int main() {
    std::string sentence;
    std::cout << "Enter a sentence: ";
    std::getline(std::cin, sentence);
    std::istringstream iss(sentence);
    int word_count = 0;
    std::string word;
    while (iss >> word) ++word_count;
    std::cout << "Word count = " << word_count << std::endl;
    return 0;
}
```

### 49. Find Sum of Digits in an Integer
```cpp
#include <iostream>
int main() {
    int num, sum = 0;
    std::cout << "Enter an integer: ";
    std::cin >> num;
    while (num != 0) {
        sum += num % 10;
        num /= 10;
    }
    std::cout << "Sum of digits = " << sum << std::endl;
    return 0;
}
```

### 50. Reverse a Number
```cpp
#include <iostream>
int main() {
    int num, reversed = 0;
    std::cout << "Enter a number: ";
    std::cin >> num;
    while (num != 0) {
        reversed = reversed * 10 + num % 10;
        num /= 10;
    }
    std::cout << "Reversed number = " << reversed << std::endl;
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
