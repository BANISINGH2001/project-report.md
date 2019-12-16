
![](https://www.muftjobs.com/wp-content/uploads/2019/08/gndec-recruitment.png)
# PROGRAMMING FOR PROBLEM SOLVING ESC -18105
 
 ## My Programs
|                         |    |
| --------------------   | --------------  |
| Submitted by           | Banipreet Singh   |
| Roll Number            | 1921017        |
| Branch                 | ITA1          |
| Submitted to           | Er. RANJODH KAUR| 
___________________________________

|## Sno.	|									|
---------|-----------------------------------------------------------------|
|  1	|Program to find the total experience of employees									|
|   2	|	Program to find whether the number is even or odd.								|
|	3|	Program to check whether the number is positive or negative.						
|	4|	Program to display the table between the range.							|
|5|		Program to display the table of user choice.							|
|6	|	Program to display the table of only even numbers between the range.	|
|	7|	Program to convert farheneit into centigrade.								|
|	8|	Program to draw pyramid.								|
|9	|	Program to check whether the number is armstrong number or not.			|
|	10|Program of a FIZZBUZZGAME.	|
|11	| Program to find sum of two numbers using scanf.	|
|12	|Program to find the average of numbers using functions.	|
|13	|Program to create simple calculator using switch.	|
|14	|Program to find the Factorial of a number.		|
|15	|Program to find the factorial of a number using recursion.		|
|16	|Program to find the factorial of a number using recursion.	|
|17	|Program to enter elements in an array and show all enen numbers.		|
|18	|Program to find greater among an array.		|
|19	|Program to display fibonacci series.		|
|20	| Program to sort array elements using selection sort.|








# Program to find the total experience of employees.

```c

#include<stdio.h>
int main()
{
int n,sum=0,exp;
printf("Enter number of employeers:");
scanf("%d",&n);
for(int i=1;i<=n;i++)
{
printf("Enter experience of %d th employeers:",i);
scanf("%d",&exp);
sum=sum+exp;
}
printf("%d\n",sum);
return 0;
}
```
# Output
```c
Enter number of employeers:3
Enter experience of 1 th employeers:5
Enter experience of 2 th employeers:3
Enter experience of 3 th employeers:4
12
```
# Program to find whether the number is even or odd.
```c
#include<stdio.h>
int main()

{
int a;

printf("\n\nENTER THE NUMBER : ");
scanf("%d",&a);

if (a%2==0)
{
printf("\n\nNUMBER IS EVEN");
}

else
{                                                                        
printf("\n\nNUMBER IS ODD\n\n");
}
return 0;
}
```
# Output
```c
ENTER THE NUMBER : 5


NUMBER IS ODD
```

# Program to check whether the number is positive or negative.
 ```c
   #include<stdio.h>
int main()
{
int a;

printf("ENTER THE NUMBER : ");
scanf("%d",&a);
if (a>0)
{
printf("NUMBER IS POSITIVE");
}
else
{
printf("NUMBER IS NEGATIVE");                                               
}                                                        
return 0;
}
```
# Output
```c
ENTER THE NUMBER : 5
NUMBER IS POSITIVE
```

# Program to display the table between the range.
```c
#include <stdio.h>
int main() {
    int n, i, range;
    printf("Enter an integer: ");
    scanf("%d", &n);
    printf("Enter the range: ");
    scanf("%d", &range);
    for (i = 1; i <= range; ++i) {
        printf("%d * %d = %d \n", n, i, n * i);
    }
    return 0;
}
```
# Output
```c
Enter an integer: 12
Enter the range: 8
12 * 1 = 12 
12 * 2 = 24 
12 * 3 = 36 
12 * 4 = 48 
12 * 5 = 60 
12 * 6 = 72 
12 * 7 = 84 
12 * 8 = 96
```

# Program to display the table of user choice.
```c
#include<stdio.h>
int main()
{
int i,j;
printf("Table of:");
scanf("%d\n",&j);

for(i=0;i<=10;i++) 
printf("%d x %d = %d\n",j,i,j*i);

return 0;
}
```
# Output
```c
Table of: 5

5 X 0 = 0
5 X 1 = 5
5 X 2 = 10
5 X 3 = 15
5 X 4 = 20
5 X 5 = 25
5 X 6 = 30
5 X 7 = 35
5 X 8 = 40
5 X 9 = 45
5 X 10 = 50
```
# Program to display the table of only even numbers between the range.
```c
#include<stdio.h>
int main()
{

        int a,b,i,j;
        printf("\nENTER THE FIRST NUMBER : ");
        scanf("%d",&a);
        printf("\nENTER THE SECOND NUMBER : ");
        scanf("%d",&b);
        for(a=a;a<=b;a++)
        {
         if(a%2==0)
         {
             for(i=0;i<=10;i++)

                {
                j=a*i;
                printf("\n%d * %d = %d\n",a,i,j);
                }
        }
}

return 0;
}
```
# Output
```c
ENTER THE FIRST NUMBER : 3

ENTER THE SECOND NUMBER : 5

4 * 0 = 0

4 * 1 = 4

4 * 2 = 8

4 * 3 = 12

4 * 4 = 16

4 * 5 = 20

4 * 6 = 24

4 * 7 = 28

4 * 8 = 32

4 * 9 = 36

4 * 10 = 40
```

# Program to convert farheneit into centigrade.
```c
#include<stdio.h>

int main()
{
 float celcius,fehrenheit;

printf("Please enter the temperature in fehrenheit: \n");
scanf("%f",&fehrenheit);
 
celcius=(fehrenheit-32)*5/9;

printf("\n %.2f fehrenheit= %.2f celcius \n", fehrenheit,celcius);

return 0;
}
```
# Output
```c
Please enter the temperature in fahrenheit: 
90

90.00 fahrenheit= 32.22 celsius 
```


# Program to draw pyramid.
```c
#include<stdio.h>
int main()
{
int n,i,j;
printf("Enter number of rows you want to print for pyramid:\n");
scanf("%d",&n);

for(i=1;i<=n;i++)
{
for(j=1;j<=2*n-1;j++)
{
if(j>=n-(i-1) && j<=n+(i-1))
printf("*");
else
printf(" ");
}
printf("\n");
}
return 0;
}
```
# Program to check whether the number is armstrong number or not.
```c
#include<stdio.h>
int main(){
int no,n,r,c,sum=0;
printf("enter  a number:\n");
scanf("%d",&n);
no=n;
while(n>0)
{
r=n%10;
c=r*r*r;
 sum=sum+c;
n=n/10;
}
if(no==sum)
printf("the given number %d is an armstrong number\n",no);
if(no!=sum)
printf("the given number %d is not an armstrong number\n",no);
return 0;
}
```
# Output
```c
enter  a number:
153
the given number 153 is an armstrong number
```
# Program of a FIZZBUZZGAME.
```C
#include <stdio.h> 
  
int main() 
{ 
    int i; 
    for (i=1; i<=100; i++) 
    { 
        // number divisible by 3 and 5 will 
        // always be divisible by 15, print  
        // 'FizzBuzz' in place of the number 
        if (i%15 == 0)         
            printf ("FizzBuzz\t");     
          
        // number divisible by 3? print 'Fizz' 
        // in place of the number 
        else if ((i%3) == 0)     
            printf("Fizz\t");                  
          
        // number divisible by 5, print 'Buzz'   
        // in place of the number 
        else if ((i%5) == 0)                        
            printf("Buzz\t");                  
      
        else // print the number             
            printf("%d\t", i);                  
  
    } 
  
    return 0; 
} 
```
# Output
```C
1    2    Fizz    4    Buzz    Fizz    7    8    Fizz    Buzz    11   
Fizz    13    14    FizzBuzz    16    17    Fizz    19    Buzz    
Fizz    22    23    Fizz    Buzz    26    Fizz    28    29    FizzBuzz    
31    32    Fizz    34    Buzz    Fizz    37    38    Fizz    Buzz    41    
Fizz    43    44    FizzBuzz    46    47    Fizz    49    Buzz    Fizz    
52    53    Fizz    Buzz    56    Fizz    58    59    FizzBuzz    61    
62    Fizz    64    Buzz    Fizz    67    68    Fizz    Buzz    71    
Fizz    73    74    FizzBuzz    76    77    Fizz    79    Buzz    Fizz    
82    83    Fizz    Buzz    86    Fizz    88    89    FizzBuzz    91    
92    Fizz    94    Buzz    Fizz    97    98    Fizz    Buzz    
```
# Program to find sum of two numbers using scanf.
```c
#include<stdio.h>
 
int main()
{
   int a, b, sum;
 
   printf("\nEnter two no: ");
   scanf("%d %d", &a, &b);
 
   sum = a + b;
 
   printf("Sum : %d", sum);
 
   return(0);
}
```
# Output
```c
Enter two no: 5 6
Sum : 11
```
# Program to find the average of numbers using functions.
```c
#include <stdio.h>
float average(int a, int b){
    return (float)(a+b)/2;
}
int main()
{
    int num1, num2;
    float avg;

    printf("Enter first number: ");
    scanf("%d",&num1);
    printf("Enter second number: ");
    scanf("%d",&num2);

    avg = average(num1, num2);

    //%.2f is used for displaying output upto two decimal places
    printf("Average of %d and %d is: %.2f",num1,num2,avg);

    return 0;
}
```
# Output
```c
Enter first number: 20
Enter second number: 13
Average of 20 and 13 is: 16.50
```
# Program to create simple calculator using switch.
```c
#include <stdio.h>
 
int main()
{
    int num1,num2;
    float result;
    char ch;    //to store operator choice
     
    printf("Enter first number: ");
    scanf("%d",&num1);
    printf("Enter second number: ");
    scanf("%d",&num2);
     
    printf("Choose operation to perform (+,-,*,/,%): ");
    scanf(" %c",&ch);
     
    result=0;
    switch(ch)    
    {
        case '+':
            result=num1+num2;
            break;
             
        case '-':
            result=num1-num2;
            break;
         
        case '*':
            result=num1*num2;
            break;
             
        case '/':
            result=(float)num1/(float)num2;
            break;
             
        case '%':
            result=num1%num2;
            break;
        default:
            printf("Invalid operation.\n");
    }
 
    printf("Result: %d %c %d = %f\n",num1,ch,num2,result);
    return 0;
}
```
# Output
```c
First run:
    Enter first number: 10
    Enter second number: 20 
    Choose operation to perform (+,-,*,/,%): +
    Result: 10 + 20 = 30.000000 
   
```
# Program to find the Factorial of a number.
```c
#include <stdio.h>
 
int main()
{
  int c, n, f = 1;
 
  printf("Enter a number to calculate its factorial\n");
  scanf("%d", &n);
  for (c = 1; c <= n; c++)
    f = f * c;
 
  printf("Factorial of %d = %d\n", n, f);
 
  return 0;
}
```
# Output
```c
Enter a number to calculate its factorial
6
Factorial of 6 = 720
```
# Program to find the factorial of a number using recursion.

```c
#include<stdio.h>
int find_factorial(int);
int main()
{
   int num, fact;
   //Ask user for the input and store it in num
   printf("\nEnter any integer number:");
   scanf("%d",&num);
 
   //Calling our user defined function
   fact =find_factorial(num);
 
   //Displaying factorial of input number
   printf("\nfactorial of %d is: %d",num, fact);
   return 0;
}
int find_factorial(int n)
{
   //Factorial of 0 is 1 
   if(n==0)
      return(1);
 
   //Function calling itself: recursion
   return(n*find_factorial(n-1));
}
```
# Output
```c
Enter any integer number: 4
factorial of 4 is: 24
```
# Program to enter elements in an array and show all enen numbers.
```c
 #include <stdio.h>
    void main()
    {
 
        int array[100], i, num;
        printf("Enter the size of an array \n");
 
        scanf("%d", &num);
        printf("Enter the elements of the array \n");
 
        for (i = 0; i < num; i++) 
        {
            scanf("%d", &array[i]);
        }
 
        printf("Even numbers in the array are - ");
        for (i = 0; i < num; i++) 
        {
            if (array[i] % 2 == 0) 
            {
                printf("%d \t", array[i]);
            }
        }
return 0;
}
```
# Output
```c
Enter the size of an array
6
Enter the elements of the array
12
19
45
69
98
23
Even numbers in the array are - 12     98
```
# Program to find greater among an array.
```c

#include <stdio.h>
 
int main()
{
 
        int array[50], size, i, largest;
 
        printf("\n Enter the size of the array: ");
	scanf("%d", &size);
 
        printf("\n Enter %d elements of  the array: ", size);
 
        for (i = 0; i < size; i++)
		scanf("%d", &array[i]);
 
        largest = array[0];
 
        for (i = 1; i < size; i++) 
        {
		if (largest < array[i])
			largest = array[i];
	}
 
        printf("\n largest element present in the given array is : %d", largest);
 
        return 0;
 
}
```
# Output
```c
Enter the size of the array: 5
 
Enter 5 elements of  the array: 12
56
34
78
100
 
largest element present in the given array is : 100
```
# Program to display fibonacci series.
```c
#include<stdio.h>    
int main()    
{    
 int n1=0,n2=1,n3,i,number;    
 printf("Enter the number of elements:");    
 scanf("%d",&number);    
 printf("\n%d %d",n1,n2);//printing 0 and 1    
 for(i=2;i<number;++i)    
 {    
  n3=n1+n2;    
  printf(" %d",n3);    
  n1=n2;    
  n2=n3;    
 }  
  return 0;  
 }
 ```
 # Output
 ```c
 Enter the number of elements:15
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377
```
# Program to sort array elements using selection sort.
```c
#include <stdio.h>
int main()
{
int a[100], n, i, j, position, swap;
printf("Enter number of elementsn");
scanf("%d", &n);
printf("Enter %d Numbersn", n);
for (i = 0; i < n; i++)
scanf("%d", &a[i]);
for(i = 0; i < n - 1; i++)
{
position=i;
for(j = i + 1; j < n; j++)
{
if(a[position] > a[j])
position=j;
}
if(position != i)
{
swap=a[i];
a[i]=a[position];
a[position=swap;
}
}
printf("Sorted Array:n");
for(i = 0; i < n; i++)
printf("%dn", a[i]);
return 0;
}
```
# Output
```c
Enter number of elements 
4
Enter 4 numbers 
4
2
7
1
Sorted array:
1
2
4
7
```
