# EX 34 C program to read a file name from user and create that file and insert student roll numbers in to that file.
## DATE:
## AIM:
To write a C program to read a file name from user and create that file and insert student roll numbers in to that file.

## Algorithm

1.Declare a file pointer, a character array for the file name, and variables for number of students and roll numbers.

2.Read the file name from the user and open the file using fopen() in write mode "w".

3.Check if the file pointer is NULL; if so, display an error message and terminate the program.

4.Read the number of student roll numbers and use a loop to input each roll number and write it into the file using fprintf().

5.Close the file using fclose() and display a success message.

## Program:
```
#include <stdio.h>

int main() {
    FILE *fp;
    char a[100];
    int n, roll;
    scanf("%s", a);

    fp = fopen(a, "w");

    if (fp == NULL) {
        printf("Error! Unable to create file.\n");
        return 1;
    }
    scanf("%d", &n);

    for (int i = 0; i < n; i++) {
        scanf("%d", &roll);
        fprintf(fp, "%d\n", roll); 
    }

    
    fclose(fp);

    printf("%s Opened\n", a);
    printf("Data added Successfully\n");

    return 0;
}

```

## Output:

<img width="547" height="300" alt="Screenshot 2026-03-19 185429" src="https://github.com/user-attachments/assets/61a61ee6-af3a-4853-a1a1-ffd2dc95931b" />


## Result:
Thus the program was executed and the output was verified successfully.
