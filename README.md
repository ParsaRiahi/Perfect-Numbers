# Perfect-Numbers

#include <stdio.h>

int main(void)
{
    int x;
    int y;
    int z = 0;

    printf("Enter a number: ");
    scanf("%d", &x);

    printf("All numbers:\n");
    for(y = 1; y < x; y++)
    {
        if(x % y == 0)
        {
            printf("%d ", y);
            z = z + y;
        }
    }
    printf("\n"); 
    printf("Combined: %d\n", z);

    if(x == z)
    {
        printf("%d is a perfect number.\n", x);
    }
    else
    {
        printf("%d is not a perfect number.\n", x);
    }

    return 0;
}
