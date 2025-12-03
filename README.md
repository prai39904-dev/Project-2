# Project-2
Calculator
#include <stdio.h>

int main() {
    char op;
    float a, b;

    printf("Enter operator (+ - * /): ");
    scanf(" %c", &op);

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    if (op == '+')
        printf("Result = %.2f\n", a + b);
    else if (op == '-')
        printf("Result = %.2f\n", a - b);
    else if (op == '*')
        printf("Result = %.2f\n", a * b);
    else if (op == '/') {
        if (b != 0)
            printf("Result = %.2f\n", a / b);
        else
            printf("Cannot divide by zero\n");
    }
    else
        printf("Invalid operator\n");

    return 0;
}
