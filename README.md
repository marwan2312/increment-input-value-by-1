#include <stdio.h>

// Function declaration
void edit(int *num);

int main() {
    int x;
    
    printf("Enter a value for x: ");
    scanf("%d", &x);
    
    printf("Before edit: x = %d\n", x);

    edit(&x);

    printf("After edit: x = %d\n", x);

    return 0;
}

void edit(int *num) {
    (*num)++;
}
