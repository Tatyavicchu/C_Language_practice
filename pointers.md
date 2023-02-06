#  POINTERS

`-` A variable which stores the memory address of another variable.

### `-` CODE 1.1
```c
#include<stdio.h>
int main(){
int star= 5; \\ star a variable to store a variable.
int *ptr =&age; \\  * -> value at address.
int moon=*ptr; \\   storing the value of ptr in  
return 0;
}
```

### Declaring pointers
 `-` int *ptr
 
 `-` float *ptr
 
 `-` char *ptr

### Format specifier to print address 
`-` printf("%p",&age);    OR   printf("%u",&age);

`NOTE:`  the diffrence between '%p' and '%u' is that both of them print address of a variable but '%p' prints hexadecimal value address of a variable and '%u' prints unsigned                 integer address value of the variable.  



`-` for example:  
```c
  printf("%p",&age);  \\ output= 0X 7ffe853db8dc
  printf("%u",&age);   \\ output= 370592044 -> both are the same address but since above one is hard to read so this one is used for user compatibility.
```

### Format specifier to print value at address
`-` printf("%d",age);   OR 

`-` printf("%d",*(&age);  OR      

`-` printf("%d",*ptr);


## Pointer to pointer
```c
 int age=22;
 int*ptr=&age;
 int ** pptrr=&ptr;
```

