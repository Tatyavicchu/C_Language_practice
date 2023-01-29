# FUNCTION

Function is a subprogram within a program which does a particular task not multiple.
A program has minimum of a single fuction which is main function. Main fuction has a pre-defined name but its defination is user defined.

```c
  1 ->  void helloworld(){
        defination of the function.
        
        
           void= return type.
        helloworld=name of the fuction or function declaration.
        
        }
  
 ```
 ### code 1.1
 ```c

 #include<stdio.h>
void namaste(){
  printf("namaste\n");
}
void bonjour(){
  printf("bonjour");
}
int main(){
  char x;
  printf("entert he nationality: ");
  scanf("%c",&x);
  if(x=='i'){
    namaste();
  }
  else if(x=='f'){
    bonjour();
  }
  return 0;  
}
 ```
 ### code 1.2
 ```c
     #include<stdio.h>
int sum(int j, int m){
  int sum= j+m;
  return sum;
}
int main(){
  int a,b;
  printf("enter the value value of numbers:  ");
  scanf("%d",&a);
  scanf("%d",&b);
   int s=sum(a,b);
  printf("%d",s);
  return 0;  
}
 ```


## Types of function

### 1->  library function or pre-defined function
     for example printf(),scanf().
### 2->  user defined function
      user defined function is named by the user and the defination is also given by the user.
      
  `a` -> function without  arguments and without return type.
   ```c              
                  void function(){}
   ```            
  `b` -> function without argument and with return type.
   ```c          
             int or float or char function(){}
   ```
  `c` -> function with argument and with return type.
   ```c        
            int or float or char  function(int a , int b){} 
   ```
  `d` -> function with arguments and without return type.
  ```c
             void function(int a, int b){}
  ```    
## Passing Arguments
 `NOTE:`  
     Without return type means it does not give any value into the main function but it is only used for printing.
   
 ` NOTE :` the variable passed from the main function is called ARGUMENT and to the variable to which it gets passed is called PARAMETER.   
             In code 1.2 (a,b) is the argument and (j,m) is the parameter.
             
             
 # RECURSION
 
 `-`  A function calling itself is called recursion.
 
 `-` Anything that can be done with iteration or loops can be done with recursion and vice-versa.
 
 `-` Base case is the condition which stops the recursion.
 
 `-` Iteration has infinite loops but recursion has stack overflow.
 
    
