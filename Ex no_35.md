# EX 35 C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
## DATE:
## AIM:
To write a C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.

## Algorithm

1.Declare a file pointer variable.

2.Open (or create) the file "Hospital.txt" using fopen() in write mode "w".

3.Check whether the file pointer is NULL to handle file creation errors.

4.If the file is created successfully, display messages indicating file creation and opening.

5.Close the file using fclose() and display a message indicating successful closure.

## Program

```
#include <stdio.h>

int main() {
    FILE *fp;
    fp = fopen("Hospital.txt", "w");

    if (fp == NULL) {
        printf("Error! Unable to create file.\n");
        return 1; 
    }

    printf("File Created Successfully\n");
    printf("File Opened\n");

   
    fclose(fp);

    printf("File Closed\n");

    return 0;
}

```

## Output:

<img width="505" height="167" alt="Screenshot 2026-03-19 185811" src="https://github.com/user-attachments/assets/6cec6e50-7db7-462f-bcc2-0fad2ee0a247" />



## Result:
Thus the program was executed and the output was verified successfully.
