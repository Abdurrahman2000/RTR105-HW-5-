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
