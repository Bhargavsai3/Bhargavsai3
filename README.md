#include <stdio.h>

int main (void)
{
    int i, j, k;

    int N = 4;

    for(i=1; i<=N; i++) 
    {
        for(j=(N*2)-(i*2); j>=1; j--)
            printf(" ");

        for(j=1, k=i; j<=(i*2)-1; j++)
        {
            printf("%d", k);

            if(j>=i)
                k++;
            else
                k--;
        }

        printf("\n");
    }

    for(i=N-1; i>=1; i--) 
    {
        for(j=(N*2)-(i*2); j>=1; j--)
            printf(" ");

        for(j=1, k=i; j<=(i*2)-1; j++)
        {
            printf("%d", k);

            if(j>=i)
                k++;
            else
                k--;
        }

        printf("\n");
    }

    return 0;
}
