#include <stdio.h>
int main (){
int num;
printf("Please eneter data type- 1 -int 2 -long long 3 -char: \n");

scanf("%d",&num);
if(num<=1)
{
int i=1,f=1,num;
printf("Enter your number: \n");

scanf("%d",&num);
for(i<=num;f=f*i;i++)
}
printf("Factorial of %d is: %d",num,f);
}
if(num<=2)
{
long long i=1,f=1,num;
printf("Enter your number : \n");

scanf("%lld",&num);
for(i<=num;f=f*i;i++)
}
rintf("Factorial of %lld is: %lld",num,f);
}
if(num<=3)
{
char i=1,f=1,num;
printf("Enter your number : \n");

scanf("%hhd",&num);
for(i<=num;f=f*i;i++)
}
printf("Factorial of %hhd is: %hhd",num,f);
return 0;
}
}
