#Scientific Calculator 
#include <stdio.h>
#include <math.h>

int main() {
    int choice;
    double a, b;

    printf("===== Scientific Calculator =====\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("5. Square Root\n");
    printf("6. Power\n");
    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            printf("Enter two numbers: ");
            scanf("%lf %lf", &a, &b);
            printf("Result = %.2lf", a + b);
            break;

        case 2:
            printf("Enter two numbers: ");
            scanf("%lf %lf", &a, &b);
            printf("Result = %.2lf", a - b);
            break;

        case 3:
            printf("Enter two numbers: ");
            scanf("%lf %lf", &a, &b);
            printf("Result = %.2lf", a * b);
            break;

        case 4:
            printf("Enter two numbers: ");
            scanf("%lf %lf", &a, &b);
            if(b != 0)
                printf("Result = %.2lf", a / b);
            else
                printf("Division by zero is not possible.");
            break;

        case 5:
            printf("Enter a number: ");
            scanf("%lf", &a);
            printf("Square Root = %.2lf", sqrt(a));
            break;

        case 6:
            printf("Enter base and exponent: ");
            scanf("%lf %lf", &a, &b);
            printf("Result = %.2lf", pow(a, b));
            break;

        default:
            printf("Invalid Choice");
    }

    return 0;
}
