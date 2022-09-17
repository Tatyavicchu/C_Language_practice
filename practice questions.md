# Questions


### `Question 1` ->  Write a program to print the average of two numbers.

  ```c
  #include <stdio.h>
# include<math.h>
 int main() {
  int a; int b; int c;
   printf("enter number a :");
     scanf ("%d", &a);
   printf("enter number b :");
   scanf ("%d", &b);
    printf("enter number c :");
    scanf ("%d", &c);
   int power;
   power= (a+b+c)/3;
   printf("%d \n",power);
   return 0;
}
  ```
  
  
  ### `Question 2` -> write a program for pass/fail marks system
  ###                 marks<30 = fail, marks>30 = pass, marks>100 = Not valid.
  
  ```c
 #include <stdio.h>
# include<math.h>
  int main() {
    int marks;
  
  printf("enter your marks(1-100)  :");
   scanf("%d",&marks);
    // marks>30? printf("pass") :printf("fail");
   if(marks<=30){
     printf("fail");
   }
   else if(marks>30 && marks<=100)
   {
     printf("pass");
   }
   else{
     printf("not valid");
   }
   return 0;
}
}
  ```

|sno|name|solution|
|-|-|-|
|[c++](https://github.com/Tatyavicchu/C_Language_practice/edit/main/practice%20questions.md)|fhg|
