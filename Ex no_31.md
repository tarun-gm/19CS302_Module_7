# EX 31 C program to find the biggest among three numbers using structure
## DATE:
## AIM:
To write a C program to find the biggest among three numbers using structure

## Algorithm

1.Start the program and define a structure to store three integers a, b, and c.

2.Declare a structure variable and read values for a, b, and c.

3.Assume the first value (a) as the largest and store it in max.

4.Compare b and c with max and update max if a larger value is found.

5.Display the largest value and stop the program.

## Program:
```
#include<stdio.h>
typedef struct
{
    int a,b,c;
    
}num;
int main()
{
    num n;
    
    scanf("%d%d%d",&n.a,&n.b,&n.c);
    int max=n.a;
    if(n.b>max)max=n.b;
    if(n.c>max)max=n.c;
    printf("%d\n",max);
}
```

## Output:

<img width="325" height="217" alt="Screenshot 2026-03-19 184119" src="https://github.com/user-attachments/assets/7b7b93a0-fa4e-4bb2-848d-09e8f4c470ee" />


## Result:
Thus the program was executed and the output was verified successfully.
