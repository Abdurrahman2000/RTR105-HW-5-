# RTR105
//Code for input of 400,000 and 100,000 and output of multiple of 2 number


#include <stdio.h>

int main ()

{  double a,b;

printf(" Input 400,000 : \n ");
scanf("%le", &a);
printf( " Input 100,000 : \n");
scanf("%le",&b);
printf("Multiple of 2 numbers entered :  %le\n ",a*b);

return 0;


}

Bitshift function code
#include<stdio.h>
int  main ()
{
char c,d,e;
char a,b;
printf("Enter a number\n");
scanf("%c",&c);
printf("Amount of bits to shift to right : ");
scanf("%c\n",&d);
printf("Amount of bits to shift to left : ");
scanf("%c\n",&e);
a = c >> d ;
b = c << e;
printf("The number you entered : %c \n",c);
printf("Result with bit-shift to right : %c\n",a);
printf("Result with bitshift to the left : %c\n",b);

return 0;
}
