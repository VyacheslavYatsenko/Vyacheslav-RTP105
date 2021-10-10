#include <stdio.h>

void main()
{
    int n;
    long long bin = 0;
    int j,rem, i = 1;

    printf("Enter a decimal number: ");
    scanf("%d", &n);


    for(j=n;j!=0;j)
    {
        rem = j % 2;
        j /= 2;
        bin += rem * i;
        i *= 10;
    }

    printf("%d in decimal = %lld in binary",n,bin);
}
---------------------------------------------------
#include <stdio.h>
#include <math.h>
#include <stdlib.h>

#define D 10

int main()
{
	int i, n, k, vet[D];
   
	printf("FROM DECIMALS TO BINARIES\nEnter decimal: ");
	scanf("%d", &n);
   
	k = 0;
   
	while (n != 0)
	{
		if ((n % 2) == 1) 
			vet[k] = 1;
		else
			vet[k] = 0;
          
		n /= 2;
       
		k++;
	}
	
	printf("Transformed into binary: ");
    
	for(i = k - 1; i >= 0; i --)
		printf("%d", vet[i]);
		
	printf("\n\n");
    
	system("pause");
}
