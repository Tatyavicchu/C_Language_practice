# FILE HANDLING

`1->` `file is a collection of data saved in the secondary memory.`


## Modes
`r` //open an existing file for eading only.
`w` //open an existing file for writing or editing. if an existing file is opened then previous data will be deleted.
`a` //
`r+` //
`w+` //
`rh+` //
`wh+` //
## Operations on a file.
### `1->` `Opening a file` 
```c
int main(){
FILE*ptr=fopen("filename tobe opened","mode");  // ptr is pointer of FILE data type.
return 0;
}
```
