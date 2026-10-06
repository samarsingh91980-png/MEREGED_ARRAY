#include <stdio.h>

int main() {
    int a[100], b[100], c[200];
    int n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter elements of first array:\n");
    for(i = 0; i < n; i++) {
        scanf("%d", &a[i]);
        c[i] = a[i];
    }

    printf("Enter elements of second array:\n");
    for(i = 0; i < n; i++) {
        scanf("%d", &b[i]);
        c[n + i] = b[i];
    }

    printf("Merged array:\n");
    for(i = 0; i < 2 * n; i++) {
        printf("%d ", c[i]);
    }

    return 0;
}
