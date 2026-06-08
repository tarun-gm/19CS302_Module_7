# EX 32 Program in C to read and print the product details with expiry date using nested structure.
## DATE:
## AIM:
To write a C Program to read and print the product details with expiry date using nested structure.

## Algorithm

1.Define a structure Product with members: id, product name, price, and a nested structure Date_Exp for expiry date (dd, mm, yyyy).

2.Declare a variable of type struct Product.

3.Read product details from the user (id, name, price, and expiry date).

4.Store the input values in the respective structure members.

5.Display the product details along with the expiry date in the required format.

## Program:
```
/*
#include <stdio.h>

struct Product {
    int id;
    char Product_name[50];
    float price;
    struct Date_Exp {
        int dd;
        int mm;
        int yyyy;
    } doj;
};

int main() {
    struct Product e1;
    scanf("%d", &e1.id);
    scanf("%s", e1.Product_name);   
    scanf("%f", &e1.price);
    scanf("%d", &e1.doj.dd);
    scanf("%d", &e1.doj.mm);
    scanf("%d", &e1.doj.yyyy);
    printf("product id : %d\n", e1.id);
    printf("product name : %s\n", e1.Product_name);
    printf("product name : %.2f\n", e1.price);
    printf("product date of expiry (dd/mm/yyyy) : %d/%d/%d\n",
           e1.doj.dd, e1.doj.mm, e1.doj.yyyy);

    return 0;
}


```

## Output:

<img width="895" height="373" alt="Screenshot 2026-03-19 184659" src="https://github.com/user-attachments/assets/82b89dfd-967f-42e8-9430-d3818776e84d" />


## Result:
Thus the program was executed and the output was verified successfully.
