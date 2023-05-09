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
# POINTERS IN FUNCTION CALL
`1` call by value.(all the prevoiusly used function were call by function cause we passed a value in the argument.)

`2` call by refrence.(in this the argument passed is the address of a variable.)
### `-` Code  1.2
    Swap of two numbers with the help of a third variable.
```c
   #include<stdio.h>
void swap(int *x, int *y){
 int z=*x;
  *x=*y;
  *y=z;
  printf("%d %d\n",*x,*y);
}
int main(){
  int a, b;
  printf("enter the two numbers : ");
  scanf("%d%d",&a,&b);
  swap(&a,&b);
  printf("%d %d",a,b);
  return 0;
}
```
## Pointer to Constant

`a pointer to a constant is a pointer that can be changed to point to a different memory location, but the value of the object it points to cannot be modified. To declare a pointer to a constant, the const keyword is placed before the type of the object being pointed to`

```c
int x = 10;
const int* ptr = &x; // pointer to constant int
*ptr = 20; // invalid, the value of the object being pointed to cannot be modified
ptr = &y; // valid, ptr can be changed to point to a different memory location

```
## Constant Pointer
`A constant pointer is a pointer whose value (i.e., the memory address it points to) cannot be changed once it is initialized. However, the object that it points to can be modified. To declare a constant pointer, the const keyword is placed before the type of the object being pointed to.`

```c
int x = 10;
int y = 20;
int* const ptr = &x; // constant pointer to int
*ptr = 30; // valid, modifies the value of x
ptr = &y; // invalid, ptr is a constant pointer and its value cannot be changed.
```
