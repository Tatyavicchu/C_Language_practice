# STRUCTURES
 `A collection of values of diffrent data types.`
 
 `structure is an user defined data types which can hold multiple types of data type.`

### `Syntax`
 ```c
 struct student{
 char name[100];
 int roll;
 float cgpa;
 } ; // statement terminator(;) is necessary.
 ```
 
 ### `define`
 ```c
 struct students s1;
 s1.cgpa=7.5;
 s1.name=mohit;
 s1.roll=39;
 ```

 ### `for example CODE 1.1`
 ```c
 #include<stdio.h>
#include<string.h>
struct student{   // "struct student" is the data type.
int roll;
  char name[1000];   // name ,roll and cgpa are the properties of student variable.
  float cgpa;
};
int main()
{
  struct student x;    // "x" is the variable name.
  x. roll=39;  // '.' is used to access the property of roll.
  strcpy(x.name,"mohit"); // instead of x.name strcpy() function is used to copy string to x.name because if used x.name it wont be able to update its value.
  x.cgpa=7.5;
  printf("%d\n%s\n%f",x.roll,x.name,x.cgpa);
  return 0;
}
 ```
### ARRAY OF STRUCTURES
```c
struct student x[100];
```
### `how to access`
```c
x[0].roll=200;
```

### Nesting of structures
```c
struct pokemon{
int power;
float health;
char name;
};
struct superpokemon{
int ability;
struct pokemon x;
};
```
## `use of typedef`

`typedef is used to rename the existing or new data type`.

```c
#include<stdio.h>
#include<string.h>
typedef int number; renaming "int" by "number". both int and number can be used.
int main(){
number x;
scanf("%d",&x);
printf("%d",x);
return 0;
}

```

### `typedef in structures`

```c

```
