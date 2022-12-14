 ##  W.A.P to find a input number is whether a prime number or not.
 
```c
#include<stdio.h>
#include<math.h>
int main(){
 int i,factor,n,count =0;
  printf("enter the number : ");
  scanf("%d",&n);
  for(int i=2;i%2==0;i++){
    if(n%i==0){
    count=1;
      }
    }
  if(count ==0){
    printf(" prime number");
  }
    else{
      printf("non prime number");
    }
  
  return 0;
}
```
