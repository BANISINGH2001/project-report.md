
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
# Program to find whether the number is even or odd.
```c
#include<stdio.h>
int main()
{

int  num;
printf("Enter any number:");
scanf("%d",&num);

if (num%2==0)
printf("Given number %d is Even \n",num);
else
printf("Given number %d is Odd \n",num);

return 0;
}
```
 # Program to check whether the number is positive or negative.
 ```c
    #include<stdio.h>

int main()
{

int num;
printf("Enter any number: \n");
scanf("%d",&num);

if(num>0)
printf("%d is positive number \n",num );

else if(num<0)
printf("%d is negative number \n",num );

else
printf("You have entered value zero \n");

return 0;
}
```
```c
#include<stdio.h>
int main()
{
int last;
printf("Enter number:");
scanf("%d",&last);
int prime,range=0;
for(int a=2;a<last;a++)
{
 prime=0;
  for(int i=2;i<last;i++)
  {
if(last%i==0)
{
prime=prime+1;
printf("No\n");
break;
}
}
if(prime==0)
{
printf("Yes\n");
break;
}
break;
}
return 0;
}
```
# Program to display the table between the range.
```c
#include<stdio.h>
int main()
{
int n,i,range;
printf("Table of:");
scanf("%d",&n);
printf("Enter the  range:");
scanf("%d",&range);

for(i=1;i<=range;++i)
{
printf("%d X %d = %d\n",n,i,n*i);
}
return 0;
}
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
# Program to display the table of only even numbers between the range.
```c
#include<stdio.h>
int main()
{
int i,j;
printf("Table of:");
scanf("%d\n",&j);
if(j%2==0)
{
for(i=0;i<=10;i++)
printf("%d X  %d  =  %d\n",j,i,j*i);
}
else
{
printf("Number is not even\n");
}

return 0;
}
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
# Program to
```c
#include<stdio.h>

int main()
{
 int n[10];
 int i,j;

 for(i=10;i<10;i++)
{
  n[i]=i+100;
}
 for(j=0;j<10;j++)
{
 printf( "Element[%d]= %d\n",j,n[j] );
}
 return 0;
}
```
# Program 
```c
#include<stdio.h>
int main()
{
 int a,b, result, n, i;
 printf("Enter the number of terms: ");
 scanf("%d", &n);

 a=0;
 b=1;

 for(i=1; i<=n; i++)
{
   printf("%d\n",a);
   result=a+b;
   a=b;
   b=result;
}
}
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

```c
#include<stdio.h>
int main(){
int  a,b,i,hcf;
printf("Enter 1st integer:\n");
scanf("%d",&a);
printf("enter 2nd intger:\n");
scanf("%d",&b);

for(int i=1;i<=a||i<=b;i++)
{
if(a%i==0 && b%i==0)
hcf=i;
}
printf("hcf=%d",hcf);

return 0;
}
```
```c
#include<stdio.h>
int main(){
int  a,b,i,lcm,gcd;
printf("Enter 1st integer:\n");
scanf("%d",&a);
printf("enter 2nd intger:\n");
scanf("%d",&b);
printf("\n");

for(int i=1;i<=a&&i<=b;i++)
{
if(a%i==0 && b%i==0)
gcd=i;
}
lcm=(a*b)/gcd;
printf("lcm=%d",lcm);

return 0;
}
```
```c
#include<stdio.h>
int main(){
int m,n,p,q;
printf("enter number of rows of 1st matrix: ");
scanf("%d",&m);
printf("enter number of columns of 1st matrix: ");
scanf("%d",&n);
printf("enter number of rows of 2nd matrix: ");
scanf("%d",&p);
printf("enter number of columns of 2nd matrix: ");
scanf("%d",&q);

if(n==p){
//for matrix 1
puts("\n\t matrix 1");
int matrix1[m][n];
// input for matrix 1
for(int i=1;i<=m;i++){
for(int j=1;j<=n;j++){
printf("enter value at %dth row and %dth column : ",i,j);
scanf("%d",&matrix1[i][j]);
}}
// output for matrix 1
puts("\nmatrix 1 is -->");
for(int i=1;i<=m;i++){
for(int j=1;j<=n;j++){
printf("%d\t",matrix1[i][j]);
if(j==n)
printf("\n");}}

//matrix 2
int matrix2[p][q];

puts("\n\t matrix 2");
// input for matrix 2
for(int k=1;k<=p;k++){
for(int l=1;l<=q;l++){
printf("enter value at %dth row and %dth column : ",k,l);
scanf("%d",&matrix2[k][l]);
}}
// output for matrix 2
puts("\nmatrix 2 is -->");
for(int k=1;k<=p;k++){
for(int l=1;l<=q;l++){
printf("%d\t",matrix2[k][l]);
if(l==q)
printf("\n");}}

//multiplication of both matrices
int matrix[m][q];
int sum=0;
//multiplication
for(int a=1;a<=m;a++){
for(int b=1;b<=q;b++){
for(int c=1;c<=p;c++){
sum =sum + matrix1[a][c]*matrix2[c][b];}
matrix[a][b]=sum;
sum=0;}}
//output for matrix 
puts("\n\t product of two matrices is -->");
for(int a=1;a<=m;a++){
for(int b=1;b<=q;b++){
printf("%d\t",matrix[a][b]);
if(b==q)
printf("\n");
}}
}
return 0;
}
```
```c
#include<stdio.h>
int main()
{
int arra[5]={1,5,8,2,7};
int c;
printf("enter the number you want to check");
scanf("%d",&c);
for(int i=0;i<5;i++)
{
if(c==arra[i])
{printf("yes");}
else
printf("no");
}
return 0;}
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
```c
#include<stdio.h>
int sum(int c);

int  main()
{

int a,b;
printf("please enter a number to calculate the sum of digits:\n");
scanf("%d",&a);
b=sum(a);
printf("%d\n",b);
}

int sum(int c)
{
int sum1=0,n;
while(c!=0)
{
sum1=sum1+c%10;
c=c/10;


}
return sum1;
}
```
```c
#include<stdio.h>
int avg(int a,int  b,int c,int d,int e);
int main()
{
int a,b,c,d,e,f;
printf("enter 5 numbers:\n");
scanf("%d %d %d %d %d",&a,&b,&c,&d,&e);
f=avg(a,b,c,d,e);
printf("avg is %d",f);
}
int avg(int a,int b,int c,int d,int e)
{
int  ans;
ans=(a+b+c+d+e)/5;
//printf("the average of entered 5 numbers %3.f %3.f %3.f %3.f %3.f is %3.f",a,b,c,d,e,ans);
return ans;
}
```
```C
#include<stdio.h>
int main()
{
int arr[10];
int i;
for(i=0;i<10;i++){
printf("Enter value of arr[%d]:",i);
scanf("%d",&arr[i]);
           }

for(i=0;i<10;i++)
        {
if(arr[i]%2==0){
printf("\n%d is even.\n",arr[i]);
                     }
}}
```
```C
#include<stdio.h>
int main(){
int a[10][10],b[10][10],mul[10][10],r,c,i,j,k;
printf("enter the number of row=");
scanf("%d",&r);
printf("enter the number of column=");
scanf("%d",&c);
printf("enter the first matrix element=\n");
for(i=0;i<r;i++)
{
for(j=0;j<c;j++)
{
scanf("%d",&a[i][j]);
}
}
printf("enter the second matrix element=\n");
for(i=0;i<r;i++)
{
for(j=0;j<c;j++)
{
scanf("%d",&b[i][j]);
}
}

printf("multiply of the matrix=\n");
for(i=0;i<r;i++)
{
for(j=0;j<c;j++)
{
mul[i][j]=0;
for(k=0;k<c;k++)
{
mul[i][j]+=a[i][k]*b[k][j];
}
}
}
for(i=0;i<r;i++)
{
for(j=0;j<c;j++)
{
printf("%d\t",mul[i][j]);
}
printf("\n");
}
return 0;
}
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
Output
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
