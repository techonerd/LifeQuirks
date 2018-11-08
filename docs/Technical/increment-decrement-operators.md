# C – Increment/decrement Operators
Increment operators are used to increase the value of the variable by one and decrement operators are used to decrease the value of the variable by one in C programs.
#### Syntax:
Increment operator: ++var_name; (or) var_name++;

Decrement operator: – -var_name; (or) var_name – -;
#### Example:
Increment operator :  ++ i ;    i ++ ;

Decrement operator :  – – i ;   i – – ;
## INCREMENT OPERATORS:
In this program, value of “i” is incremented one by one from 1 up to 9 using “i++” operator and output is displayed as “1 2 3 4 5 6 7 8 9”.
```
#include <stdio.h>
int main()
{
     int i=1;
     while(i<10)
     {
         printf("%d ",i);
         i++;
     }    
}
```
#### OUTPUT:
> 1 2 3 4 5 6 7 8 9
### PRE – INCREMENT OPERATORS:
```
#include <stdio.h>
int main()
{
           int i=0;
           while(++i < 5 )
           {
                printf("%d ",i);
           }
           return 0;
}
```
#### OUTPUT:
> 1 2 3 4

Step 1 : In above program, value of “i” is incremented from 0 to 1 using pre-increment operator.

Step 2 : This incremented value “1” is compared with 5 in while expression.

Step 3 : Then, this incremented value “1” is assigned to the variable “i”.

Above 3 steps are continued until while expression becomes false and output is displayed as “1 2 3 4”.
### POST – INCREMENT OPERATORS:
```
#include <stdio.h>
int main()
{
           int i=0;
           while(i++ < 5 )
           {
                printf("%d ",i);
           }
           return 0;
}
```
#### OUTPUT:
> 1 2 3 4 5

Step 1 : In this program, value of  i “0” is compared with 5 in while expression.

Step 2 : Then, value of “i” is incremented from 0 to 1 using post-increment operator.

Step 3 : Then, this incremented value “1” is assigned to the variable “i”.

Above 3 steps are continued until while expression becomes false and output is displayed as “1 2 3 4 5”.
## DECREMENT OPERATORS:
In this program, value of “i” is decremented one by one from 20 up to 11 using “i–” operator and output is displayed as “20 19 18 17 16 15 14 13 12 11”.
```
#include <stdio.h>
int main()
{
    int i=20;
    while(i>10)
    {
         printf("%d ",i);
         i--;
    }    
}
```
#### OUTPUT:
> 20 19 18 17 16 15 14 13 12 11
### PRE – DECREMENT OPERATORS:
```
#include <stdio.h>
int main()
{
           int i=10;
           while(--i > 5 )
           {
                printf("%d ",i);
           }
           return 0;
}
```
#### OUTPUT:
> 9 8 7 6

Step 1 : In above program, value of “i” is decremented from 10 to 9 using pre-decrement operator.

Step 2 : This decremented value “9” is compared with 5 in while expression.

Step 3 : Then, this decremented value “9” is assigned to the variable “i”.

Above 3 steps are continued until while expression becomes false and output is displayed as “9 8 7 6”.
### POST – DECREMENT OPERATORS:
```
#include <stdio.h>
int main()
{
           int i=10;
           while(i-- > 5 )
           {
                printf("%d ",i);
           }
           return 0;
}
```
#### OUTPUT:
> 9 8 7 6 5

Step 1 : In this program, value of  i “10” is compared with 5 in while expression.

Step 2 : Then, value of “i” is decremented from 10 to 9 using post-decrement operator.

Step 3 : Then, this decremented value “9” is assigned to the variable “i”.

Above 3 steps are continued until while expression becomes false and output is displayed as “9 8 7 6 5”.
### DIFFERENCE BETWEEN PRE/POST INCREMENT & DECREMENT OPERATORS:
|            Operator           |                           Description                           |
|:-----------------------------:|:---------------------------------------------------------------:|
| Pre increment operator (++i)  | value of i is incremented before assigning it to the variable i |
| Post increment operator (i++) | value of i is incremented after assigning it to the variable i  |
| Pre decrement operator (--i)  | value of i is decremented before assigning it to the variable i |
| Post decrement operator (i--) | value of i is decremented after assigning it to variable i      | 