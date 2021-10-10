#include <stdio.h>
#define CHAR_SIZE   8
#define ARRAY_SIZE sizeof(int)* CHAR_SIZE
int main()
{
    // counter for binary array
    int i = 0,j=0;
    //num for decimal number
    int num;
    //Array to store binary number
    int binaryNum[ARRAY_SIZE];
    printf("Enter decimal number: ");
    scanf("%d", &num);
    while (num > 0)
    {
        binaryNum[i] = num % 2;
        num = num / 2;
        i++;
    }
    // printing binary array in reverse order
    for (j = i - 1; j >= 0; j--)
    {
        printf("%d",binaryNum[j]);
    }
    return 0;
}
                                               -----------------------------First Trial------------------------------------------
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
--------------------------------------------------------------------------Second Trial---------------------------------------------------------------------------------------
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
-----------------------------------------------------------------------Third Trial---------------------------------------------------------------------------------------
