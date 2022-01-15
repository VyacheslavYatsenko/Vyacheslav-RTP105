#include <stdio.h>
#include <math.h>

 void main () 
 {
     int   k, n=2, b , a;
    long double eps=1.e-3, h , integr1=0., integr2, c=M_PI;
     integr2 = (b*c-a) * (sinh(a)+sinh(b*c))/n;
     printf("Please enter a- should be bigger than 0!        ");
     scanf("%d", &a);
     printf("Please enter b         ");
     scanf("%d", &b);
     
 while(fabs(integr2-integr1)>eps)
{
 n *= 2;
 h = (b*c-a)/n;
 integr1 = integr2;
 integr2 = 0.;
 for(k=0;k<n; k++)
 {
 integr2 +=h*sinh(a+(k+0.5)*h) ;
 //integr2 = integr2 +h*sin(a+k*h);
 }
}
printf ( " Integraal javeertiiba: %Lf\n" , integr2);
}
