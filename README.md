# TASK--4-CPP-COMPILER-DESIGN-BASICS
COMPANY : CODETECH IT SOLUTION PVT.LTD
NAME : SOUMITA SAHA 
INTERN ID : CTO4DN493
DOMAIN C++ PROGRAMMING 
DURATION 4 WEEKS
MENTOR :NEELA SANTOSH


This C++ program evaluates a basic arithmetic expression entered by the user. It uses two stacks—one for integers (values) and another for operators (+, -, *, /)—to compute the result.

Key Components:

1. Header Files:

iostream is used for input/output.

stack is used to store numbers and operators.

string supports string manipulation.



2. doMath() Function:
This helper function performs the actual arithmetic based on the operator passed. It supports four basic operations: addition, subtraction, multiplication, and division. It checks for division by zero to avoid a runtime error.


3. evaluate() Function:
This function processes the string input expression character by character:

It skips any spaces.

If it finds a digit, it forms the complete number (to handle multi-digit numbers) and pushes it onto the values stack.

If it finds an operator, it pops the top two numbers and the top operator, calculates the result using doMath(), and pushes the result back. This is done until the operator stack is empty.

Finally, it performs any remaining operations left in the stacks after parsing the whole expression.



4. main() Function:
This is where the program starts. It prompts the user to input a string representing an arithmetic expression (e.g., 3+4*2). It then calls the evaluate() function and prints the result.



Example:

Input: 12+3*2
The program parses and calculates the result step-by-step. However, note that this implementation does not consider operator precedence (i.e., it evaluates strictly left to right), so 12+3*2 will be evaluated as (12+3)*2 = 30 instead of the mathematically correct 12+(3*2) = 18.

Limitations:

No support for parentheses or floating-point numbers.

No proper operator precedence.

No input validation (e.g., detecting invalid expressions).


Summary:

This program demonstrates basic expression evaluation using stacks in C++, suitable for educational purposes or as a starting point for building a more advanced calculator.

OUTPUT : 
