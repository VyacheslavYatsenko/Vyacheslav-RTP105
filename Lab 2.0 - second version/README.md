#include <stdio.h>
#include <math.h>
int main (){
    float a=1*M_PI, b=-1, y , delta_y =1e-3/* 0.001 */ , funkca , funkcb , funkcy ;
 int k=0;

 funkca = asinh(a) ; funkcb = asinh(b) ;
 if ( funkca*funkcb >0){
 printf ( "Intervaalaa [%.2f ;%.2f ] arcsinh (y) funkcijai " ,a , b) ;
 printf ( " saknju nav ( vai taajaa ir paaru saknju skaits )\n" ) ;
 return 1;}

 printf ( " asinh (%7.3f)=%7.3f \t \t \t \t " ,a , asinh(a) ) ;
 printf ( " asinh (%7.3f )=%7.3f \n " ,b , asinh (b) ) ;

 while (( b-a)>delta_y ){
 k++;//k=k+1;//k+=1;
 y = (a+b) / 2;
 if ( funkca* asinh(y)>0) // pie a=0 −> funkca=0 −> reizinaajums i r p r e c i i z i 0
 //visu laiku -> v i s u l a i k a " straadaa " b=x
 a = y ;
 else
 b=y ;
 printf ( "%2d . interaacija : asinh (%7.3f )=%7.3f \t " ,k , a , asinh(a) ) ;
 printf ( " asinh (%7.3f )=%7.3f \t " ,y , asinh (y)) ;
 printf ( " asinh (%7.3f )=%7.3f \n" ,b , asinh (b));}

 printf ( "Saakne atrodas pie x=%.3f , jo asinh (y) ir %3f \n" ,y , asinh ( y ) ) ;

 return 0;}
