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
```c
#include<stdio.h>
int main(){
  char fullname[50];
  gets(fullname);
  puts(fullname);
  return 0;
}
```
`Note-` since gets() is dangeorus and outdated it  is replaced by fgets().
`Format of fgets()`: fgets(string name, size of the string,stdin)   // stdin= standard input.
 `-` It stops when n-1 characters are input or enter  or next line is entered.
