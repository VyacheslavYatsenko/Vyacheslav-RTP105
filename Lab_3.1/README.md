#include <stdio.h>
#include <math.h>
void main (){

int a,b;
double dx, f1_x, fx, x;

//float y;
printf("Please enter number a:      ");
scanf("%d", &a);
printf("Please enter number b:      ");
scanf("%d", &b);
printf("Please enter the value of precesion   \n");
scanf("%lf", &dx);
printf("       x               sinh(x)      F1_sinh'(x)     F2_Sinh'(x)   F1_Sinh''(x)      F2_Sinh''(x) \n");
x = a;
while(x<b){
    // y=sinhx);
    fx = sinh(x);
    f1_x= cosh(x);
    printf("%10.2f \t %10.2f \t %10.2f \t %10.2f \t %10.2f \t %10.2f \n", x,sinh(x), f1_x ,sinh(x), cosh(x),sinh(x));
    //printf("%10.2f\t%10.2f\n",x,y);
    x = x + dx ; //x = x + dx;
}
}
