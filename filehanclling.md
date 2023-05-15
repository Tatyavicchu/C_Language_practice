# FILE HANDLING

`1->` `file is a collection of data saved in the secondary memory.`


## Modes
`r` //open an existing file for eading only.

`w` //open an existing file for writing or editing. if an existing file is opened then previous data will be deleted.

`a` // opens an existing or creates a new file and then add the new data in it without deleting the previous one. 

`r+` //this mode will open a new file for read and writing.

`w+` // open a text file for both reading and writng. It creates a new file and if a the file does exist then it first shorteb the file to zero length.

`a+` // opens a new text file if it does not exist but if it exist the reading starts from the start but the appending starts from the end.


# File functions in programming.
### `fputs`  `->` to insert a string in file. // fputs(string,file pointer);    
 ```c
 #include<stdio.h>
#include<string.h>
#include<stdlib.h>

int main(){
 FILE* ptr=fopen("filehandlingin c.txt","r");
 if(ptr!=EOF){
    fputs("hello wolrd",ptr);
 }
return 0;
}

 ```
 
 ### `fputc`  `->` to insert a character in file.  //fputc(character,file pointer);
 ```c
 #include<stdio.h>
#include<string.h>
#include<stdlib.h>

int main(){
 FILE* ptr=fopen("filehandlingin c.txt","r");
 if(ptr!=EOF){
    fputc("h",ptr);
 }
return 0;
}

 ```
 
 
 ### `fgets`  `->` to get a string form the file to the console. //fgets(file pointer);
 ```c
 
 ```
 
 ### `fgetc`  `->` to get a character form the file to the console. //fgetc(file pointer);
 ```c
 #include<stdio.h>
#include<string.h>
#include<stdlib.h>

int main(){
char str[100];
 FILE* ptr=fopen("filehandlingin c.txt","r");
 if(ptr!=EOF){

     char c=fgetc(ptr);
     printf("%c",c);
 }
return 0;
}

 ```
 
 ### `fprintf`  `->`

 ### `fscanf`  `->`
 

