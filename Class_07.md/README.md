#include <stdio.h>
int main (){
int num;
printf("Please eneter data type- 1 -int 2 -long long 3 -char: \n");

scanf("%d",&num);
if(num<=1)
{
int i=1,f=1,num;
printf("Enter your number and data type: \n");

scanf("%d",&num);
while(i<=num){
f=f*i;
i++;
}
printf("Factorial of %d is: %d",num,f);
return 0;
}
if(num<=2)
{
long long i=1,f=1,num;
printf("Enter your number : \n");

scanf("%lld",&num);
hile(i<=num){
f=f*i;
i++;
}
printf("Factorial of %lld is: %lld",num,f);
return 0;
}
if(num<=3)
{
char i=1,f=1,num;
printf("Enter your number : \n");

scanf("%hhd",&num);
while(i<=num){
f=f*i;
i++;
}
printf("Factorial of %hhd is: %hhd",num,f);
return 0;
}
}
