# conditional statements are used to run certain part of code according to the output of condition
## -> there are two types of conditional statements
     -> else/if conditional statements
     -> switch conditional statements
  ### - If/ Else conditional statements
        In this type of statments only two conditioln is possible.
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
         this is the shortcut for the "if/else" conditional statement but only two conditions will be made.
                   
                 "  condition? do something if TRUE : do something if FALSE;  "
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
 ### -  Switch conditionl statements
        in this type of conditonal statements multiple conditions can be made.
        
  ## Syntax
   ```c
        #include <stdio.h>
    # include<math.h>
 int main() {
   char date; //A seminar cs; B seminar b; C seminar c
   printf("enter availibility date(A-C) :");
   scanf("%c",& date);

   switch(date){
     case'A' : printf("you are available for seminar cs join at 3am ");
                  break;
     case 'B': printf("you are available for seminar cs join at 2AM ");
                  break;
      case 'C': printf("you are available for seminar cs join at noon");
                  break;
     default :   printf(" cant join");
   }

   
   return 0;
   }
   ```
###    Conditions for switch operators :
    
   ->  cases can be in any order
   ->  Nested switch( switch inside switch or if/else inside of condition) are allowed.
