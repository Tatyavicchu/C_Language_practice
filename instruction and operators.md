# there are different types of operator in c 
- ## Arithmetic Operator
  - `+` -> to add two numbers 
  - `-` -> to subtract two numbers
  - `*` -> to multiply two numbers
  - `/` -> to divide two numbers
  - `%` -> to get remainder of two numbers
    - ### NOTE: '%' does not work with decimal numbers
  - `pow` -> function used to find power of two numbers
 ## Syntax
   ```c
 #include <stdio.h>
 int main() {
 int a= 5, b=2;
   int power= pow(a,b);
   printf("%d",power);
   return 0;
   }
   ```
- ## Conversion 

- #### this is of two type one is IMPLICIT and other is EXPLICIT.
- IMPLICIT conversion is done by compiler himself but EXPLICIT conversion is done by us and the compiler is forced to do it.


## Operator precedence
 - this is the operator's order like BODMASS in mathematics.
    - `a` -> '/' , '%' 
    - `b` -> '+' , '-' 
    - `c` -> '=' 
   ### NOTE : - If two operators of same precedence are present in the program then solution should be done by left to right.
      ###      - If a bracket is present, first solve the bracket and then continue as told above.
      
