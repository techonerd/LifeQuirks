---
title: Basics of Programming
---
# **Basics of Programming**
I will be using C language to demonstrate nuances shared nearly all the programs.
# Section
- [Data types](#Data-types)
- [Functions](#Functions)
- [Operators](#Operators)
## Data types
Data type determines the type of data a variable will hold. If a variable x is declared as int. it means x can hold only integer values. Every variable which is used in the program must be declared as what data-type it is. 
### Primitive Data Types
These data types are offered by programming language.
#### Integer | int
Integer data type represents all integers (all negative and positive numbers including 0)

   int a = 2; int b = -200;

#### Character | char
Characters represent english alphabets and special symbols.
Characters have corresponding integer codes, search for ASCII codes for more details.

   char a = 'b'; char dollar = '$';

#### Float | float
Float are used to store decimal values with single precision.
Double are used to store decimal values with single precision with double precision.

The word double derives from the fact that a double-precision number uses twice as many bits as a regular floating-point number.
For example, if a single-precision number requires 32 bits, its double-precision counterpart will be 64 bits long.
Source - [Stack Overflow Question](https://stackoverflow.com/questions/801117/whats-the-difference-between-a-single-precision-and-double-precision-floating-p#801146)
### Derivative Data Types
Derived data types are nothing but primary datatypes but a little twisted or grouped together like array, stucture, union and pointer.
#### Arrays
Arrays are reffered to as structured data types. An array is defined as [finite](alt-text:-finite-means-data-range-must-be-defined.) [ordered](alt-text:-ordered-means-data-must-be-stored-in-continuous-memory-addresses.) collection of [homogenous](alt-text:-homogenous-means-data-must-be-of-similar-data-type.) data, stored in contiguous memorylory locations.

Arrays can be used in following kind of scenerios,

- to store list of Employee or Student names,
- to store marks of students,
- or to store list of numbers or characters etc.
## Functions
Functions are great way avoid copy pasting code. It allows programmers to break logic into small pieces and execute them in efficient manner.

In C Programming, As per our requirement, We can define the User defined functions in multiple ways

- Function with no argument and no Return value
- Function with no argument and with Return value
- Function with argument and No Return value
- Function with argument and Return value

      From the above, 1 and 3 types does not return any value when the function is called so, We use void return type while defining the function.

      When we call the function 2 and 4 types will return some value, We have to use the appropriate data type (int, float, double etc) as return type while defining the function. We use return keyword inside the function to return some value when the function is called from the main() function or any sub functions.
For detailed explaination on types of funtions, refer to the [types of fuction](./types-of-functions.md) file.
## Operators
Operators allow us to perform different kinds of operations on [operands](https://en.wikipedia.org/wiki/Operand). An operator is a symbol that tells the compiler to perform a certain mathematical or logical manipulation.

C operators can be classified into following types:

- [Arithmetic operators](#Arithmetic-Operators) (+,-,/,*,%)
- [Relational operators](#Relational-operators) (==,!=,>,<,>=,<=)
- [Logical operators](#Logical-operators) (&&,||, !)
- [Bitwise operators](#Bitwise-operators) (&, |, ^, ~, >>,<<)
### Arithmetic Operators: 
These are used to perform arithmetic/mathematical operations on operands. The binary operators falling in this category are:
#### Addition: 
The ‘+’ operator adds two operands. 
```
int a = 2; int b = 3; int c = a+b;
c=5
```
#### Subtraction:
The ‘-‘ operator subtracts two operands. 
```
int a = 3; int b = 2; int c = a-b;
c=1
```
#### Multiplication: 
The ‘*’ operator multiplies two operands. 
```
int a = 2; int b = 3; int c = a*b;
c=6
```
#### Division: 
The ‘/’ operator divides the first operand by the second. 
```
int a = 6; int b = 3; int c = a/b;
c=2
```
#### [Modulus](https://en.wikipedia.org/wiki/Modulus): 
The ‘%’ operator returns the remainder when first operand is divided by the second. 
```
int a = 3; int b = 2; int c = a%b;
c=1
```
The ones falling into the category of [unary](https://en.wikipedia.org/wiki/Unary_operation) arithmetic operators are:
#### Increment: 
  The ‘++’ operator is used to increment the value of an integer. When placed before the variable name (also called pre-increment operator), its value is incremented instantly. 
 ```
 int a = 5;
 ++a;          //a becomes 6
 ```
  And when it is placed after the variable name (also called post-increment operator), its value is preserved temporarily until the execution of this statement and it gets updated before the execution of the next statement. 
#### Decrement: 
  The ‘–-‘ operator is used to decrement the value of an integer. When placed before the variable name (also called pre-decrement operator), its value is decremented instantly. 
 ```
 int a = 5;
--a;          //a becomes 6 
 ```
  And when it is placed after the variable name (also called post-decrement operator), its value is preserved temporarily until the execution of this statement and it gets updated before the execution of the next statement. 

 For a better understanding of pre & post increment and decrement operators, refer to increment and decrement operators  [explaination](./increment-decrement-operators.md) page.
### Relational Operators:
Relational operators are used for comparison of two values. Let’s see them one by one:
#### Equals | ==
‘==’ operator checks whether the two given operands (inputs) are equal or not. If so, it returns true. Otherwise it returns false.
```
int a = 2; int b = 3; int c = 2;
a == b // False
c == a // True
```
#### Not Equals | !=
‘!=’ operator checks whether the two given operands are equal or not. If not, it returns true. Otherwise it returns false. It is the exact boolean complement of the ‘==’ operator. 
```
int a = 2; int b = 3; int c = 2;
a != b // True
c != a // False
```
#### Greater than | >
‘>’ operator checks whether the first operand is greater than the second operand. If so, it returns true. Otherwise it returns false.
```
int a = 2; int b = 3; int c = 2;
a > b // False
b > c // True
```
#### Less than | <
‘<‘ operator checks whether the first operand is lesser than the second operand. If so, it returns true. Otherwise it returns false.
```
int a = 2; int b = 3; int c = 2;
b < a // False
c < b // True
```
#### Greater than or Equals | >=
‘>=’ operator checks whether the first operand is greater than or equal to the second operand. If so, it returns true. Otherwise it returns false.
```
int a = 2; int b = 3; int c = 2;
a >= b // False
c >= a // True
b >= c // True
```
#### Less than or Equals | <=
‘<=’ operator checks whether the first operand is lesser than or equal to the second operand. If so, it returns true. Otherwise it returns false. 
```
int a = 2; int b = 3; int c = 2;
b <= a // False
c <= a // True
c <= b // True
```
### Logical Operators:
They are used to combine two or more conditions/constraints or to complement the evaluation of the original condition in consideration. The result of the operation of a logical operator is a boolean value either true or false. They are described below:
#### Logical AND: 
  The ‘&&’ operator returns true when both the conditions in consideration are satisfied. Otherwise it returns false. 
```
int a = 0; int b = 3; int c = 2;
a && b // False
b && c // True
```
#### Logical OR: 
  The ‘||’ operator returns true when one (or both) of the conditions in consideration is satisfied. Otherwise it returns false. 
```
int a = 0; int b = 0; int c = 2;
a || b // False
b || c // True
```
#### Logical NOT: 
  The ‘!’ operator returns true when the condition in consideration is not satisfied. Otherwise it returns false. 
```
int a = 0; int b = 3; int c = 2;
a != b // True
b != c // False
```
### Bitwise operators 
Bitwise operator is used to perform bit-level operations on the operands. The operators are first converted to bit-level and then calculation is performed on the operands. The mathematical operations such as addition , subtraction , multiplication etc. can be performed at bit-level for faster processing.

In C, following are some bitwise operators (work at bit-level)
#### (bitwise AND) & 
  Takes two numbers as operands and does AND on every bit of two numbers. The result of AND is 1 only if both bits are 1.
#### (bitwise OR) |
  Takes two numbers as operands and does OR on every bit of two numbers. The result of OR is 1 any of the two bits is 1.
#### (bitwise XOR) ^
  Takes two numbers as operands and does XOR on every bit of two numbers. The result of XOR is 1 if the two bits are different.

*Truth Table for bitwise operator &, | and ^*
```
|  a  |  b  |  a & b  |  a|b  | a ^ b |
| ----------------------------------- |
|  0  |  0  |    0    |   0   |   0   |
|  0  |  1  |    0    |   1   |   1   |
|  1  |  0  |    0    |   1   |   1   |
|  1  |  1  |    1    |   1   |   0   |
```
#### (left shift) << 
  Takes two numbers, left shifts the bits of the first operand, the second operand decides the number of places to shift.
#### (right shift) >> 
  Takes two numbers, right shifts the bits of the first operand, the second operand decides the number of places to shift.
```
a = 0001000
b = 2
a << b = 0100000 
a >> b = 0000010 
```