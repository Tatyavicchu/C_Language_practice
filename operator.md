# there are different types of operator in c 
- ## Arithmetic Operator
  - `+` -> to add two numbers 
  - `-` -> to subtract two numbers
  - `*` -> to multiply two numbers
  - `/` -> to divide two numbers
  - `%` -> to get remainder of two numbers
    - ### NOTE: '%' does not work with decimal numbers
  - `pow` -> function used to find power of two numbers
  - ```c
  ### Example
 #include <stdio.h>
 int main() {
 int a= 5, b=2;
   int power= pow(a,b);
   printf("%d",power);
   return 0;
   ```
- ## logical operators
  - `&&` -> and 
