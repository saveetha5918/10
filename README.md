#include <stdio.h>

int main() {
    int num, binary = 0, place = 1;

    printf("Enter a decimal number: ");
    scanf("%d", &num);

    // Convert decimal to binary
    while(num > 0) {
        binary += (num % 2) * place;
        num /= 2;
        place *= 10;
    }

    printf("Binary number: %07d\n", binary);  // Print binary number with leading zeroes

    return 0;
}
