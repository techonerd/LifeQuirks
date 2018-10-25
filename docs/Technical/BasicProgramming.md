---
title: Basics of Programming
---

# Basics of Programming

I will be using C language to demonstrate nuances shared nearly all the programs

## Primitive Data Types

These data types are offered by programming language.

### Integer | int

Integer data type represents all integers (all negative and positive numbers including 0)

```C
int a = 2; int b = -200;
```

### Character | char

Characters represent english alphabets and special symbols.
Characters have corresponding integer codes, search for ASCII codes for more details.

```C
char a = 'b'; char dollar = '$';
```

### Float | float

Float are used to store decimal values with single precision.
Double are used to store decimal values with single precision with double precision.

The word double derives from the fact that a double-precision number uses twice as many bits as a regular floating-point number.
For example, if a single-precision number requires 32 bits, its double-precision counterpart will be 64 bits long.
Source - [Stack Overflow Question](https://stackoverflow.com/questions/801117/whats-the-difference-between-a-single-precision-and-double-precision-floating-p#801146)

## Functions

Functions are great way avoid copy pasting code. It allows programmers to break logic into small pieces and execute them in efficient manner

### Method Signature
