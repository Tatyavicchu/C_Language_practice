# conditional statements are used to run certain part of code according to the output of condition
## -> there are two types of conditional statements
  ### - If/ Else conditional loops
        In this type of loop only two conditioln is possible.
 ```c
// if( condition ){
// executes if conditon is true
// always put condition in (condition) bracket
// }
// else{
// executes if condition is false
// }

// example
int a = 4;

if(a<5)
{
  printf("yes");
  
}
else {
printf("no");
}
```
## NOTE :
       To add multiple condition use else if.
```c
#include <stdio.h>
# include<math.h>
 int main() {
 int age;
  printf("enter age \n");
   scanf("%d",&age);
   if (age<18)
   {
     printf("teen");
   }
     else if(age== 18)
     {
       printf("eighteen");
     }
   else
  {
     printf("adult");
   }
   return 0;
}
```
## S/C Ternary operator
         this is the shortcut for the "if/else" loop.
         
            condition? do soomething if TRUE : do something if FALSE;
   ```c
    #include <stdio.h>
#include<math.h>
 int main() {
 int age;
  printf("enter age \n");
   scanf("%d",&age);
   
age>18? printf("adult/n") :printf("teen");
   
   return 0;
}
        ```
 ### -  Switch conditionl loops
        in this type of conditonal looop multiple conditions can be made.

