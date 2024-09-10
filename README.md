# C-programming

#include <stdio.h>

int main() {
    int num, sum = 0, digit;
    printf("Enter an integer: ");
    scanf("%d", &num);
    // Calculate the sum of digits
    while (num != 0) {
        digit = num % 10;  // Get the last digit
        sum += digit;      // Add the digit to the sum
        num /= 10;         // Remove the last digit
    }
    // Output the result
    printf("Sum of digits: %d\n", sum);
    return 0;
}
