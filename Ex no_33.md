# EX 33 C program to read a file name from user and create that file using fopen().
## DATE:
## AIM:
To write a C program to read a file name from user and create that file using fopen().

## Algorithm

1.Declare a file pointer and a character array to store the file name.

2.Read the file name from the user using scanf().

3.Open (or create) the file using fopen() in write mode "w".

4.Check if the file pointer is NULL to handle errors in file creation.

5.If successful, display messages for file creation, opening, and closing, then close the file using fclose().  

## Program:
```
#include <stdio.h>

int main() {
    FILE *fp;
    char a[20];
    scanf("%s",a);
    fp = fopen(a, "w");

    if (fp == NULL) {
        printf("Error! Unable to create file.\n");
        return 1; 
    }
    

    printf("%s File Created Successfully\n",a);
    printf("%s File Opened\n",a);

   
    fclose(fp);

    printf("%s File Closed\n",a);

    return 0;
}

```

## Output:

<img width="844" height="319" alt="Screenshot 2026-03-19 185204" src="https://github.com/user-attachments/assets/de888692-81a9-40bb-96a5-abdf8911bb25" />


## Result:
Thus the program was executed and the output was verified successfully.
