# ARRAY
`-`  A collection of similar data in the memory is called array.
## Pointer Arithmetic
`-` pointers can be incremented and decremented.

`-` Pointers can be substracted.

`-` We can also compare two pointers. The result wil be in binary showing true(1)/false(0).
 
`-` pointers can be used in an array as the following example :
## `Code 1.1` 
```c
#include<stdio.h>
int main(){
int n,i,x;
printf("enter the size of the array : ");
scanf("%d",&n);
int arr[n];
for( i=0;i<n;i++){
 scanf("%d",&arr[i]);

} 
  printf("enter the value of x : ");
  scanf("%d",&x);
  int *ptr=&arr[x];
  ptr++;  \\ here increment is done by 1 but the value will not increase by 1, it wil increase by the size int=4  / float=8 / char=1 takes in the memory.
  printf("%d\n",*ptr); 
  return 0;
}
```
### `-` Array is a pointer
## `code 1.2`
```c
#include<stdio.h>
int main(){
int arr[]={29,30,78,87,876};
  int*ptr=arr;
  int*pointer=&arr[0];
  printf("%d %d",*pointer ,*ptr); \\output=29 29
  return 0;
}
```
### Array as function argument
`-` Array can be passed  to a diffrent function from main function.

`declaration` :
```c
void declaration(int arr[],int n)  // where n is the size of array.
```
### Multidimensional array
`Declaration`
```c
int arr[rows][coloums]={{12,34} ,{43,54}};
```
