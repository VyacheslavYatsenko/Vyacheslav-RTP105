#include <stdio.h>
#include <math.h>
void main (){
    
    int a,b;
    float  delta_x=1.e-2, x ;
    //float y;
    printf("Please enter number a:      ");
    scanf("%d", &a);
    printf("Please enter number b:      ");
    scanf("%d", &b);
    printf("\tx\t\tsinh(x) \tsin\'(x)\t\tsin\''(x)\n");
    x = a;
    while(x<b){
        // y=sinhx);
        printf("%10.2f\t%10.2f\t%10.2f\n", x ,sinh(x) ,(sinh(x + delta_x)-sinh(x))/delta_x);
        //printf("%10.2f\t%10.2f\n",x,y);
        x+= delta_x; //x = x + delta_x;
    }
}        
