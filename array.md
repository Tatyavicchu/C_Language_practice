# ARRAY
`-`  A collection of similar data in the memory is called array.
## Pointer Arithmetic
`-` pointers can be incremented and decremented.
`-` pointers can be used in an array as the following example :
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
  ptr++;  \\ here increment is done by 1 but the value will not increase by 1, it wil increase by the size int=4  / float=8 / char=8 takes in the memory.
  printf("%d\n",*ptr); 
  return 0;
}
```
