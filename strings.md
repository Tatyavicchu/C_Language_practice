# STRINGS
`-` It is a character array which ends with a null character('\0').

`-` null characters denotes string termination.
### `example: CODE 1.1`
```c
#include<stdio.h>
int main(){
  char chara[]="mohit";
  char name[]={'M','O','H','I','T','\0'};
  for(int i=0;chara[i]!='\0';i++){
  printf("%c",chara[i]);// output=mohit (but not as a word ).
    }printf("\n");
  for(int i=0;chara[i]!='\0';i++){
    printf("%c",name[i]); // output=MOHIT(not as a word).
    }
  return 0;
}
```
### format specifier
```c
printf("%s",chara);  // output = mohit(as a word).
scanf("%s",chara);  // '&' is not used because string name is already an pointer.
```
`NOTE :` scanf cannot take input of multiple characters with spaces between them. For example : mohit bhandari. Hence use gets() & puts(). 
### gets()/puts()
## `code 1.2`
```c
#include<stdio.h>
int main(){
  char fullname[50];
  gets(fullname);
  puts(fullname);
  return 0;
}
```
`Note-` since cgets() is dangeorus and outdated it  is replaced by fgets().

`Format of fgets()`: fgets(string name, size of the string,stdin)   // stdin= standard input.

`-` It stops when n-1 characters are input or enter  or next line is entered.

## `code 1.3`
 ```c
 #include<stdio.h>
int main(){
  char fullname[50];
  fgets(fullname,50,stdin);
  puts(fullname);
  return 0;
}
 ```
 # Standard library functions -> #include<string.h>
### `1` strlen()
```c
 strlen(string) -> counts number of the characters in a string excluding '\0'.
 ```
### `for example: Code 1.4`
```c
 #include<stdio.h>
#include<string.h>
int main(){
  char ch[]="mohit";
  int length=strlen(ch);  // here strlen() gives us a unsigned long value which is then typecasted into integer value. 
  printf("%d",length);
  return 0;
}
```

### `2` strcpy()
```c
strcpy(new string,old string) -> this copies the old string into the new string but does not change/update the old string.
```
### `for example : code 1.5`
```c
#include<stdio.h>
#include<string.h>

int main(){
  char str1[]="hello";
  char str2[]= "world";
  strcpy(str1,str2);
  puts(str1);
  return 0;
}
```
### `2` strcat()
```c
strcat(new string,old string) -> this ccombines the two strings.
```
### `for example: code 1.6`
```c
#include<stdio.h>
#include<string.h>

int main(){
  char str1[10000]="hello";
  char str2[600]= "world";
  strcat(str1,str2);
  puts(str1);
  return 0;
}
```
