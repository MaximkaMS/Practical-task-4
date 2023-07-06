# Practical-task-4
#include <stdio.h>

int countEqualDivisors(int n) {
    int count = 0;
    int i;

    for (i = 1; i <= n; i++) {
        if (n % i == n / i) {
            count++;
        }
    }

    return count;
}

int main() {
    int n;

    printf("Введіть натуральне число n: ");
    scanf("%d", &n);

    int result = countEqualDivisors(n);

    printf("Кількість рівних дільників числа %d: %d\n", n, result);

    return 0;
}
