# program-6d
C module 6
EXP.No:6d-Positive or negative using calloc().

Date: 26/03/26
Name: JADEN SAMUEL ABRAHAM
Ref no: 25003451

AIM:
To write a C program to find whether the  given number is positive or negative using calloc().

ALGORITHM:

Declare a pointer variable using calloc() to dynamically allocate memory for one integer.
Read a number from the user and store it in the allocated memory.
Check the value stored:
	•	If the number is greater than 0 → print “Positive number”
	•	If the number is less than 0 → print “Negative number”
	•	Else → print “Number is Zero”
Free the allocated memory using free().

PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *num;

    // Allocate memory for one integer using calloc
    num = (int *)calloc(1, sizeof(int));

    if (num == NULL) {
        printf("Memory not allocated.\n");
        return 1; // Exit if memory allocation fails
    }

    // Input number
    printf("Enter a number: ");
    scanf("%d", num);

    // Check whether the number is positive, negative or zero
    if (*num > 0)
        printf("The number is Positive.\n");
    else if (*num < 0)
        printf("The number is Negative.\n");
    else
        printf("The number is Zero.\n");

    // Free allocated memory
    free(num);

    return 0;
}
```
OUTPUT:

Enter a number: 25
The number is Positive.


RESULT:

Thus the C program to find whwther the given number is positive or negative using calloc() is successfully executed.

















