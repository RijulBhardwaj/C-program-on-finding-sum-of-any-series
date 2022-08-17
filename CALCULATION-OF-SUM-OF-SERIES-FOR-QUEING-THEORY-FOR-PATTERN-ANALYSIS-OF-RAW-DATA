#include <stdio.h>
#include <math.h>
int main() { 

int type ;
printf("if the progression is arithmatic in nature press 1\n if proggression is geometric in nature press 2 \n if proggrssion is harmonic in nature press 3 \n if series is of the form (1 + 1/2 + 1/3 + 1/4 + ... + 1/N) press 4 \n if series is of the form (1^2 + 2^2 + …. + n^2) press 5 \n if series is of the form (1^3 + 2^3 + 3^3 + … + n^3) press 6 \n if series is cos(x) press 7 \nplease enter input:");
scanf("%d",&type);
switch(type){
    /* the Sum of A.P Series */
    case 1 :
{
     int a, d, n, i, tn;
     int sum = 0;
 
     printf("Enter the first term value of the A.P. series: ");
     scanf("%d", &a);
     printf("Enter the total numbers in the A.P. series: ");
     scanf("%d", &n);
     printf("Enter the common difference of A.P. series: ");
     scanf("%d", &d);
     sum = (n * (2 * a + (n - 1)* d ))/ 2;
     tn = a + (n - 1) * d;
     printf("Sum of the A.P series is: ");
     for (i = a; i <= tn; i = i + d )
     {
          if (i != tn)
               printf("%d + ", i);
          else
               printf("%d = %d ", i, sum);
     }
    
}
break;
/*  the Sum of G.P Series*/
 
case 2 :

{
    float a, r, i, last_term, sum = 0;
    int n;
 
    printf("Enter the first term of the G.P. series: ");
    scanf("%f", &a);
    printf("Enter the total numbers in the G.P. series: ");
    scanf("%d", &n);
    printf("Enter the common ratio of G.P. series: ");
    scanf("%f", &r);
    sum = (a *(1 - pow(r, n + 1))) / (1 - r);
    last_term = a * pow(r, n - 1);
    printf("last_term term of G.P.: %f", last_term);
    printf("\n Sum of the G.P.: %f", sum);
}
break ;
/* the Sum of H.P Series*/
case 3 :
{
    int n;
    float i, sum, term;
 
    printf("1 + 1 / 2 + 1 / 3 +......+1 / n \n");
    printf("Enter the value of n \n");
    scanf("%d", &n);
    sum = 0;
    for (i = 1; i <= n; i++)
    {
        term = 1 / i;
        sum = sum + term;
    }
    printf("the Sum of H.P Series is = %f", sum);
}
break;
/*the Sum of Series 1 + 1/2 + 1/3 + 1/4 + ... + 1/N */
case 4 : 
{
    double number, sum = 0, i;
 
    printf("\n enter the number ");
    scanf("%lf", &number);
    for (i = 1; i <= number; i++)
    {
        sum = sum + (1 / i);
        if (i == 1)
            printf("\n 1 +");
        else if (i == number)
            printf(" (1 / %lf)", i);
        else
            printf(" (1 / %lf) + ", i);
    }
    printf("\n The sum of the given series is %.2lf", sum);
}

break ;
/* the sum of series 1^2 + 2^2 + …. + n^2. */
case 5 :
{
    int number, i;
    int sum = 0;
 
    printf("Enter maximum values of series number: ");
    scanf("%d", &number);
    sum = (number * (number + 1) * (2 * number + 1 )) / 6;
    printf("Sum of the above given series : ");
    for (i = 1; i <= number; i++)
    {
        if (i != number)
            printf("%d^2 + ", i);
        else
            printf("%d^2 = %d ", i, sum);
    }
}
break;
 
case 6 :
{
    int number, i;
    int sum = 0;
 
    printf("Enter the maximum values of series n: ");
    scanf("%d", &number);
    sum = pow(((number * (number + 1) ) / 2),2);
    printf("Sum of the series : ");
    for (i = 1; i <= number; i++)
    {
        if (i != number)
            printf("%d^3 + ", i);
        else
            printf("%d^3 = %d ", i, sum);
    }
}
break ;

case 7 :
{
    int n, x1, i, j;
    float x, sign, cosx, fact;
 
    printf("Enter the number of the terms in a series\n");
    scanf("%d", &n);
    printf("Enter the value of x(in degrees)\n");
    scanf("%f", &x);
    x1 = x;
	/*  Degrees to radians */
    x = x * (3.142 / 180.0);
    cosx = 1;
    sign = -1;
    for (i = 2; i <= n; i = i + 2)
    {
        fact = 1;
        for (j = 1; j <= i; j++)
        {
            fact = fact * j;
        }
        cosx = cosx + (pow(x, i) / fact) * sign;
        sign = sign * (-1);
    }
    printf("Sum of the cosine series = %7.2f\n", cosx);
    printf("The value of cos(%d) using library function = %f\n", x1,
    cos(x));
}
break;
default :
printf("Incorrect input");
break;
}
}
