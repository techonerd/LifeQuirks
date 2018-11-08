---
title: Types of Functions
---
# Types of Functions in C Programming
The Following examples will explain you the available function types in C programming.
- [**Function with no argument and no Return value**](#Function-with-no-argument-and-no-Return-value)
- [**Function with no argument and with Return value**](#Function-with-no-argument-and-with-Return-value)
- [**Function with argument and No Return value**](#Function-with-argument-and-No-Return-value)
- [**Function with argument and Return value**](#Function-with-argument-and-Return-value)
## Function with No argument and No Return value
In this method, We won’t pass any arguments to the function while defining, declaring or calling the function. This type of functions will not return any value when we call the function from main() or any sub function. When we are not expecting any return value but, we need some statements to be printed as output then, this type of functions are very useful.
#### CODE
In this program, We are going to calculate the Sum of 2 integer values and print the output from the user defined function itself.
```
/* Function with No argument and No Return value Example */
#include<stdio.h>

// Function Declaration
void Addition();        

void main()
{
  printf("\n ............. \n");
  
  Addition();                      
}

void Addition()
{
  int Sum, a = 10, b = 20;  
  Sum = a + b;
  
  printf("\n Sum of a = %d and b = %d is = %d", a, b, Sum);
}
```
#### OUTPUT
``` 
.............

Sum of a = 10 and b = 20 is = 30
``` 
#### ANALYSIS
If you observe the main() function, We haven’t passed any arguments /parameters to the function Addition()
Within the Addition() function,

We declared the integer variables of sum, a, b and we assigned 10 to a and 20 to b.

In the next line we calculate the sum using Arithmetic operator ( + )
```
Sum = a + b
    = 10 + 20
    = 30
```
Below printf statement is used to print the output.
```
printf("\n Sum of a = %d and b = %d is = %d", a, b, Sum);
```
Whenever we call the Addition() function then it will print the same output because the values of a and b are fixed inside the function.

## Function with no argument and with Return value
In this method, We won’t pass any arguments to the function while defining, declaring or calling the function. This type of functions will return some value when we call the function from main() or any sub function. Data Type of the return value will depend upon the return type of function declaration. For instance, if the return type is int then return value will be int.
#### CODE
In this program, We are going to calculate the multiplication of 2 integer values using the user defined function without arguments and return keyword.
```
#include<stdio.h>

int Multiplication();        

int main()
{
  int Multi;

  Multi = Multiplication();
  printf("\n Multiplication of a and b is = %d \n", Multi );        

  return 0;            
}

int Multiplication()
{
  int Multi, a = 40, b = 40;  
  
  Multi = a * b;

  return Multi;
}
```
#### OUTPUT
```
Multiplication of a and b is = 1600
```
#### ANALYSIS
If you observe the main() function,

We declared the integer variable Multi and we assigned it to the return value of the Multiplication() function because, user defined function also return integer value only.
```
Multi = Multiplication();
```
We haven’t passed any arguments /parameters to the function Multiplication()

In the next line, printf statement is used to print the output
```
printf("\n Multiplication of a and b is = %d \n", Multi);
```
Whenever we call the Multiplication() function then it will print the above statement.

Within the Multiplication() function,

We declared the integer variables of Multi, a, b and we assigned 40 to a and 40 to b.

In the next line we Multiplied both a and b using Arithmetic operator ( * )
```
Multi = a * b
      = 40 * 40
      = 1600
```
Whenever we call the Multiplication() function then it will print the same output because the values of a and b are fixed inside the function.
## Function with argument and No Return value
If you observe the above 2 methods, No matter how many times you executive, it will give the same output. We don’t have any control over the values of the variables a and b because they are fixed values. In real time, we mostly deal with dynamic data means we have to allow the user to enter his own values rather than fixed ones.

This method allows us to pass the arguments to the function while calling the function. But, This type of functions will not return any value when we call the function from main() or any sub function.

If we want to allow our user to pass his own data to the function arguments but we are not expecting any return value then, this type of functions are very useful.
#### CODE
This program allows the user to enter 2 integer values and then, We are going to pass those values to the user defined function to calculate the sum.
```
#include<stdio.h>

void Addition(int, int);        

void main()
{
  int a, b;

  printf("\n Please Enter two integer values \n");
  scanf("%d %d",&a, &b);

  //Calling the function with dynamic values
  Addition(a, b);
}

void Addition(int a, int b)
{
  int Sum;  
  
  Sum = a + b;

  printf("\n Additiontion of %d and %d is = %d \n", a, b, Sum);
}
```
#### OUTPUT
```

 Please Enter two integer values
90
40

 Additiontion of 90 and 40 is = 130
```
#### ANALYSIS
If you observe the main() function, We declared the integer variables a and b.

This program allows the user to enter 2 integer values as a and b.
```
 printf("\n Please Enter two integer values \n");
 scanf("%d %d",&a, &b);
```
In the next line, we called the Addition (int a, int b) function with the user entered values
```
 Addition(a, b);
```
Within the Addition (int a, int b) function,
We declared the integer variables of Sum and also we have integer (a, b) arguments in the function. This means, this function will allow the user to pass 2 integer values.

In the next line we added both a and b using Arithmetic operator ( + )
```
Sum = a + b;
```
In the next line, printf statement is used to print the output
```
printf("\n Additiontion of %d and %d is = %d \n", a, b, Sum);
```
## Function with argument and Return value
This method allows us to pass the arguments to the function while calling the function. This type of functions will return some value when we call the function from main() or any sub function. Data Type of the return value will depend upon the return type of function declaration. For instance, if the return type is int then return value will be int.

This type of user defined functions are called as fully dynamic function means, it provide maximum control to the end user.
#### CODE
This program allows the user to enter 2 integer values and then, We are going to pass those values to the user defined function to multiply those values and return the value using return keyword.
```
#include<stdio.h>

int Multiplication(int, int);        

int main()
{
  int a, b, Multi;

  printf("\n Please Enter two integer values \n");
  scanf("%d %d",&a, &b);

  //Calling the function with dynamic values
  Multi = Multiplication(a, b);

  printf("\n Multiplication of %d and %d is = %d \n", a, b, Multi);        
  return 0;            
}

int Multiplication(int a, int b)
{
  int Multi;  

  Multi = a * b;

  return Multi;
}

```
#### OUTPUT
~~~
 Please Enter two integer values
 60
 30

  Multiplication of 60 and 30 is = 1800
~~~
#### ANALYSIS
If you observe the main() function, We declared the integer variables Multi, a and b.

This program allows the user to enter 2 integer values as a and b.
```
printf("\n Please Enter two integer values \n");

scanf("%d %d",&a, &b);
```
In the next line, we assigned the return value of the Multiplication(int a, int b) function to the Multi integer because, user defined function also return integer value only.
```
 Multi = Multiplication(a, b);
```
We passed the user inputs as the arguments /parameters to the function Multiplication(int a, int b)

In the next line, printf statement is used to print the output
```
 printf("\n Multiplication of a and b is = %d \n", Multi);
``` 
Within the Multiplication() function,

We declared the integer variables of Multi and also we have two integer (a, b) arguments in the function. This means, this function will allow the user to pass 2 integer values.

In the next line we Multiplied both a and b using Arithmetic operator ( * ).