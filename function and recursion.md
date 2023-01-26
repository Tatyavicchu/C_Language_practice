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


## Types of function

### 1->  library function or pre-defined function
     for example printf(),scanf().
### 2->  user defined function
      user defined function is named by the user and the defination is also given by the user.
      
      -`a` -> function without  arguments and without return type.
            void function(){}
     
     b-> function without argument and with return type.
             
             int or float or char function(){}
    
    c-> function with argument and with return type.
            
            int or float or char  function(int a , int b){} 
    
    d-> function with arguments and without return type.
             void function(int a, int b){}
      
### Passing Arguments
     'note'  without return type means it does not give any value into the main function but it is only used for printing.
    
