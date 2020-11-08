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


//Code for arranging 3 input charactor in alphabetical or reverse alphabeticalorder per user's request
Please note that the user is prompted twice to confirm if to output in alphabetical or reverse due to an input-to-variable passing error in the compiling software. 

#include <stdio.h>
int
main ()
{
  char a1, b2, c3, d4, first, second, third;
  int e5, e6;
  printf ("Please enter your first charactor : ");
  scanf ("%c", &a1);
  printf ("Please enter your second charactor : ");
  scanf ("%c\n", &b2);
  printf ("Please enter your third charactor : ");
  scanf ("%c\n", &c3);
  printf
    ("For alphabetical output press 1 and enter \nFor reverse aphabetical order press 2 and enter \n");
  scanf ("%c\n", &d4);

  printf ("Entered charactors : %c %c %c %c \n", a1, b2, c3, d4);

  printf
    ("For alphabetical output press 1 and enter \nFor reverse aphabetical order press 2 and enter \n");
  scanf ("%d\n", &e5);
  first = a1;
  second = c3;
  third = d4;
//code for highest ascii value (sorting in decending order)
  if ((int) third > (int) second)
    {
      second = d4;
      third = c3;
      if ((int) d4 > (int) a1)
	{
	  first = d4;
	  second = a1;
	}
      if ((int) c3 > (int) a1)
	{
	  third = a1;
	  second = c3;
	}
    }
  if ((int) second
    >(int) first)
    {
      first = c3;
      second = a1;
      if ((int) d4 > (int) a1)
	{
	  second = d4;
	  third = a1;
	}
      if ((int) d4 > (int) c3)
	{
	  first = d4;
	  second = c3;
	}
    }

  if ((int) third > (int) first)
    {
      first = d4;
      third = a1;
      if ((int) a1 > (int) c3)
	{
	  second = a1;
	  third = c3;
	}
    }
    
    if (e5==2 || e6==2){printf("Reverse alphabetical order : %c %c %c",first,second,third);}
    if (e5==1 || e6==1){printf("Alphabetical order : %c %c %c",third,second,first);}
  return 0;
}


//Code for factorial calculation with user chosen variables (while loop)

#include <stdio.h>

int main() {
 char b1;
    printf("Enter the respective number corresponding to the variable you like to use \nchar(1)\nint(2)\nlonglong(3)\n")
    scanf("%c",&b1);
    if (b1==1)
    unsigned char a1,a2,a3,a4=1;
    {printf("Enter the number you would like to calculate factorial of - ");
    scanf("%c",&a1);
        a2=a1;
        while(a2>=2){
            a3=a3*(a2-1);
            a2-=1;}
            a4=(a1*a3);
            printf("Factorial of %c is = %c",a1,a4);}
        if  (b1==2){
              unsinged int b2,b3,b4,b5=1;
              printf("Enter the number you would like to calculate factorial of - ");
              scanf("%d",&b2);
              b3=b2;
        while (b3>=2){
                  b4=b4*(b3-1);
                  b3-=1;}
                  b5=b2*b3;
                  printf("Factorial of %d is = %d",b2,b5);}
		  if (b1==3){
            unsinged long long c1,c2,c3,c4=1;
            printf("Enter the number you would like to calculate factorial of - ");
              scanf("%",&c1);
              c2=c1;
        while (c2>=2){
            c3=c3*(c2-1);
            c2-=1;}
	    c4=c1*c3;
        printf("Factorial of % is = %",c1,c4);}
return 0;
}

//Code for factorial calculation with user chosen variables (for loop)

#include <stdio.h>

int main() {
    char b1;
    printf("Enter the respective number corresponding to the variable you like to use char(1) int(2) long long int(3)\n");
    scanf("%c",&b1);
    
    if (b1==1){
    unsigned char a1,a2,a3,a4=1;
    printf("Enter the number you would like to calculate factorial of - ");
    scanf("%c",&a1);
    if (a1==1||a1==0){printf("Factorial of %c is = 1",a1);}
        a2=a1;
        for(;a2>=2;){
            a3=a3*(a2-1);
            a2-=1;
           }
            a4=a1*a3;
            printf("Factorial of %c is = %c",a1,a4);}
        if  (b1==2){
              unsigned int b2,b3,b4,b5=1;
              printf("Enter the number you would like to calculate factorial of - ");
              scanf("%d",&b2);
              if (b2==1||b2==0){printf("Factorial of %d is = 1",b2);}
              b3=b2;
        for (;b3>=2;)
        if (b1==3){
            unsigned long long int c1,c2,c3,c4=1;
            printf("Enter the number you would like to calculate factorial of - ");
              scanf("%llu",&c1);
              if (c1==1||c1==0){printf("Factorial of %llu is = 1",c1);}
              c2=c1;
        for(;c2>=2;){
            c3=c3*(c2-1);
            c2-=1;
        }       c4=c1*c3;
        printf("Factorial of %llu is = %llu",c1,c4);
        }
        
    return 0;
}}
