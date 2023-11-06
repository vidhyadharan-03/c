# EX1(A) DATATYPES-AND-OPERATORS
## AIM:
Write a program to find sum of two integer numbers
## ALGORITHAM:
1.Start

2.Assign 2 variable of datatype integer.

3.Get input for the above 2 variables.

4.using sum opertor add both the variables.

5.Print the output on the screen.
## PROGRAM:
~~~
#include <stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    printf("Sum of %d and %d=%d",a,b,a+b);
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/27b2ecbd-1260-4aad-93e7-2bf6b5684cd1)
## RESULT:
Thus, find the sum of two integer numbers has successfully executed.


# EX1(B) CONDITIONAL-STATEMENTS
## AIM:
Write a C program to read a, b value and find the greatest value using  if-else

## ALGORITHAM:
1. Start with including header file.
2. Assign two variables a and b with integer datatype.
3. Get the Input for the above variables.
4. using IF statements check whether b is Greater than a, if yes print b.
5. Else print the value in a.
6. End the program

## PRGORAM:
~~~
#include <stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    if(b>a)
    printf("B is greatest.");
    else
    printf("A is greatest.");
    return 0 ;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/60b95dd1-eb71-4005-886f-539313a06d23)
## RESULT:
Thus, The c program has been executed successfully.

# EX1(C) OPERATORS-AND-EXPRESSIONS
## AIM:
Write a C program to calculate the area of a circle. Get the radius value from the user as an input.

## ALGORITHAM:

1.include header and math.h file to your program.

2.Declare a variable to store the radius(e.g.,radius)and a variable for the area(e.g.,area).

3.Get the input (radius value) from the user and store it in radius variable.

4.Calculate the area of the circle using the formula: area = 3.14*(pow(radius,2)).

5.Print the Area value which is stored in the area variable.

## PROGRAM:
~~~
#include <stdio.h>
#include <math.h>
int main()
{
    float a,b;
    scanf("%f",&a);
    b=3.14*(pow(a,2));
    printf("Area of circle=%.2f sq. units",b);
    return 0;
    
}
~~~

## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/27faecab-d563-4c52-adce-7be1ae0d5025)
## RESULT:
Thus, Area of circle is executed successfully.


# EX1(D) CONDITIONAL-STATEMENTS-APPLICATIONS:
## AIM:
Write a C Program to simulate arithmetic operators (+,-) using the switch statement
## ALGORITHAM:

Step 1: Include the necessary header file stdio.h.

Step 2: Declare the main function.

Step 3: Declare integer variables a, b, and c, and a character variable d.

Step 4: Read input values for a, d, and b from the user using scanf.

Step 5: Use a switch statement to handle the arithmetic operation based on the value of d.

    If d is '+', add a and b, store the result in c, and print "Result = [c]".
    If d is '-', subtract b from a, store the result in c, and print "Result = [c]".
    If d is any other character, print "Invalid Input."
    
Step 6: Use break statements to exit the switch statement.

Step 7: If none of the case conditions match, execute the default case and print "Invalid Input."
## PRGORAM:
~~~
#include<stdio.h>
int main()
{
    int a,b,c;
    char d;
    scanf("%d %c %d",&a,&d,&b);
    switch(d)
    {
        case '+':
        c=a+b;
        printf("Result = %d",c);
        break;
        case '-':
        c=a-b;
        printf("Result = %d",c);
        break;
        default :
        printf("Invalid Input");
    }
    
     
     return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/a5175291-b863-4d6d-a4a8-dca5a9065ce5)
## RESULT:
Thus, simulation of arithmetic operators using the switch statement successfully executed.


# EX2(A) LOOPS:
## AIM:
Read N as input from the user. Write a C Program to print the sum of N even numbers from 1 to N.

## ALGORITHAM:
Step 1: Include the necessary header file stdio.h. 

Step 2: Declare the main function.

Step 3: Declare an integer variable a to store user input.

Step 4: Declare an integer variable i for the loop counter.

Step 5: Initialize an integer variable sum to 0.

Step 6: Read an integer input from the user using scanf and store it in the variable a.

Step 7: Start a for loop with i initialized to 1, the loop condition i <= a, and incrementing i by 1 in each iteration.

Step 8: Inside the loop, check if i is even using if(i % 2 == 0).

Step 9: If i is even, add its value to the sum variable.

Step 10: After the loop, print the sum of even numbers using printf.

## PROGRAM:
~~~
#include<stdio.h>
int main()
{
 int a,i,sum=0;
 scanf("%d",&a);
 for(i=1;i<=a;i++)
 {
     if(i%2==0)
     sum=sum+i;
 }
 printf("Sum of even numbers from 1 to %d is %d",a,sum);
  return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/4d122fc0-29d2-4689-8250-96aa2d8061ac)
## RESULT:
Thus, printng the sum of N even numbers from 1 to N successfully executed.

# EX2(B) NESTED-LOOP:
## AIM:
Complete the C program to print rhombus  pattern

INPUT:
5
Output
    #####
   #####
  #####
 #####
#####

## ALGORITHAM:
Step 1: Include the necessary header file stdio.h.

Step 2: Declare the main function.

Step 3: Declare an integer variable a to store user input.

Step 4: Read an integer input from the user using scanf and store it in the variable a.

Step 5: Start an outer for loop to control the number of lines to be printed.

    Initialize a new integer variable i to 1.
    Set the loop condition to i <= a.
    Increment i by 1 in each iteration.

Step 6: Inside the outer loop, start an inner for loop to print spaces before # characters.

    Initialize a new integer variable j to a - i.
    Set the loop condition to j >= 1.
    Decrement j by 1 in each iteration.

Step 7: Inside the inner loop for spaces, print a space character using printf(" ").

Step 8: After the inner loop for spaces, start another inner for loop to print # characters.
Initialize a new integer variable k to 1.

    Set the loop condition to k <= a.
    Increment k by 1 in each iteration.

Step 9: Inside the inner loop for # characters, print a "#" character using printf("#").

Step 10: After both inner loops, print a newline character "\n" to move to the next line.

Step 11: The outer loop continues to the next iteration (if applicable) to create the next line of the pattern.

Step 12: Repeat steps 6 to 11 for each line until the outer loop condition is no longer satisfied.

## PROGRAM:
~~~
#include <stdio.h>

int main()
{
    int a;
    scanf("%d",&a);
    for(int i=1;i<=a;i++)
    {
        for(int j=a-i;j>=1;j--)
        {
            printf(" ");
        }
        for(int k = 1;k<=a;k++)
        {
            printf("#");
        }
        printf("\n");
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/01dfc4b8-ab2f-4a0d-9905-c5172ff152fb)
## RESULT:
Thus, The C program has been executed successfully.

# EX2(C)-FUNCTIONS:
## AIM:
Write a C program to generate Fibonacci sequence of n numbers using function, with arguments & without return type.
## ALGORITHAM:

Step 1: Include the necessary header file stdio.h.

Step 2: Declare the fibo function with the signature void fibo(int) to calculate and print Fibonacci numbers.

Step 3: Declare the main function, which is the entry point of the program.

Step 4: Declare an integer variable m to store the user input, which specifies how many Fibonacci numbers to generate.

Step 5: Use the scanf function to read an integer input from the user and store it in the variable m.

Step 6: Call the fibo function, passing the value of m as its argument. This initiates the generation of Fibonacci numbers.

Step 7: Define the fibo function, which takes an integer parameter x to determine how many Fibonacci numbers to generate.

Step 8: Inside the fibo function, declare two integer variables a and b and initialize them to 0 and 1, respectively. These variables will be used to calculate the Fibonacci sequence.

Step 9: Start a for loop with the initialization of a new integer variable i to 1, the loop condition as i <= x, and the increment of i by 1 in each iteration. This loop controls how many Fibonacci numbers are generated.

Step 10: Inside the for loop, print the current value of a using printf("%d ", a). This prints the Fibonacci numbers separated by spaces.

Step 11: Calculate the next Fibonacci number by adding a and b and store it in a new variable result.

Step 12: Update the value of a to be the previous value of b, and update the value of b to be the result. This step is essential for generating the next Fibonacci number.

Step 13: The for loop continues to the next iteration (if applicable) to generate the next Fibonacci number.

Step 14: Repeat steps 10 to 13 until the desired number of Fibonacci numbers (specified by x) is generated.

Step 15: Once the for loop is complete, the fibo function finishes its execution.

Step 16: Back in the main function, the program execution continues after the fibo function call, and the program terminates.

## POGRAM:
~~~
#include <stdio.h>
void fibo(int);
int main()
{
    int m;
    scanf("%d",&m);
    fibo(m);
    
}
void fibo(int x)
{
    int a=0,b=1;
    for(int i=1;i<=x;i++)
    {
        printf("%d ",a);
        int result = a+b;
        a=b;
        b=result;
        
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/5d90ebcd-6ae4-4434-b55d-1b25dcd554ff)
## RESULT:
Thus, Generation of Fibonacci sequence of n numbers successfully executed.

# EX2(D)-LOOPS-APPLICATIONS:
## AIM:
Write a C program for the following pattern?

12344321

123  321

12    21

1      1

## ALGORITHAM:
Step 1: Include the necessary header file stdio.h.

Step 2: Declare the main function, which is the entry point of the program.

Step 3: Declare integer variables i, j, and r. i and j will be used as loop counters, and r is initialized to 4.

Step 4: Start an outer for loop with the initialization of i to the value of r, the loop condition as i > 0, and the decrement of i by 1 in each iteration. This loop controls the number of lines to be printed.

Step 5: Inside the outer loop, start an inner for loop with the initialization of j to 1. The loop condition is j <= r, and j is incremented by 1 in each iteration. This inner loop is responsible for printing the numbers in ascending order and spaces.

Step 6: Inside the inner loop for ascending numbers, check if j is less than or equal to i. If it is, print the value of j using printf("%d", j).

Step 7: If j is greater than i, print a space character using printf(" ").

Step 8: After the first inner loop, start a second inner for loop with the initialization of j to r. The loop condition is j >= 1, and j is decremented by 1 in each iteration. This inner loop is responsible for printing the numbers in descending order and spaces.

Step 9: Inside the inner loop for descending numbers, check if j is less than or equal to i. If it is, print the value of j using printf("%d", j).

Step 10: If j is greater than i, print a space character using printf(" ").

Step 11: After both inner loops have completed, print a newline character "\n" to move to the next line, creating a new pattern line.

Step 12: The outer loop continues to the next iteration (if applicable) to create the next line of the pattern.

Step 13: Repeat steps 5 to 12 until the outer loop condition is no longer satisfied.

Step 14: Once the outer loop is complete, the program terminates.

## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int i,j,r=4;
    for(i=r;i>0;i--)
    {
        for(j=1;j<=r;j++)
        {
            if(j<=i)
            printf("%d",j);
            else
            printf(" ");
        }
        for(j=r;j>=1;j--)
        {
            if(j<=i)
            printf("%d",j);
            else
            printf(" ");
        }
        printf("\n");
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/97463a9f-cee9-4f7e-98a7-6c8437867592)
## RESULT:
Thus, the above pattern is successfully executed.

# EXP3(A)-FUNCTIONS:
## AIM:
Write a C program for a function that accepts two numbers to calculate the sum and return the total number of carries.

## ALGORITHM:
Step 1: Include the necessary header file stdio.h.

Step 2: Define the numberOfCarries function, which calculates and returns the number of carries that occur when adding two numbers digit by digit.

Step 3: Inside the numberOfCarries function, declare integer variables carry to keep track of carries, sum to store the sum of digits in the same place value, p and q to store the corresponding digits from num1 and num2, and count to keep track of the number of carries.

Step 4: Start a while loop that continues as long as both num1 and num2 are not equal to 0. This loop will process the digits from right to left.

Step 5: Within the loop, calculate p and q as the remainder when dividing num1 and num2 by 10, respectively. These represent the rightmost digits in num1 and num2.

Step 6: Calculate the sum of p, q, and the current carry value.

Step 7: Check if the sum is greater than 9, which indicates a carry. If it is, set carry to 1 and increment the count variable to keep track of the number of carries.

Step 8: If the sum is not greater than 9, set carry to 0, indicating no carry occurred.

Step 9: Update num1 and num2 by dividing them by 10, effectively removing the rightmost digits.

Step 10: Repeat steps 5 to 9 for each pair of corresponding digits in num1 and num2.

Step 11: Return the count variable, which contains the total number of carries.

Step 12: Define the main function, which is the entry point of the program.

Step 13: Declare integer variables x, y, and a to store the user inputs and the result of the numberOfCarries function.

Step 14: Use the scanf function to read integer values for x and y from the user.

Step 15: Call the numberOfCarries function, passing x and y as arguments, and store the result in the variable a.

Step 16: Print the value of a, which represents the number of carries when adding x and y.

Step 17: Return 0 to indicate successful program execution and terminate the main function.

## PRGORAM:
~~~
#include<stdio.h>
int numberOfCarries(int num1 , int num2)
{
    int carry = 0, sum, p, q, count = 0;
    while((num1!=0)&&(num2!=0))
    {
        p = num1 % 10;
        q = num2 % 10;
        sum = carry + p + q;
        if(sum>9)
        {
            carry = 1;
            count++;
        }
        else
        {
            carry = 0;
        }
        num1 = num1/10;
        num2 = num2/10;
    }
    return count;
}
int main()
{
   int x, y, a;
   scanf("%d",&x);
   scanf("%d",&y);
   a = numberOfCarries(x, y);
   printf("%d",a);
   return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/277d0d63-30c8-450d-89d2-16072b61c5ca)
## RESULT:
Thus, the c program successfully executed:


# EX3(B)-LOOPING
## AIM:
C Program to print Armstrong Numbers between 1 to n.
## ALGORITHM:
Step 1: Include the necessary header files stdio.h and math.h.

Step 2: Declare variables num, ld, digit, sum, i, and end.

Step 3: Read the upper limit end for numbers to check from the user.

Step 4: Start a for loop for i from 1 to end.

Step 5: Initialize sum to 0 for the current number.

Step 6: Set num to the current value of i.

Step 7: Calculate the number of digits in num and store it in digit.

Step 8: Enter a while loop to process digits of num from right to left.

Step 9: Calculate ld as the rightmost digit of num.

Step 10: Calculate the sum of ld raised to the power of digit and add it to sum.

Step 11: Update num by removing the rightmost digit.

Step 12: Check if i is equal to sum. If yes, it's an Armstrong number.

Step 13: Print the result if i is an Armstrong number.

Step 14: The for loop continues to the next number.

Step 15: Repeat steps 5 to 14 for all numbers from 1 to end.

Step 16: The program terminates once the for loop is complete.

## PROGRAM:

~~~
#include<stdio.h>
#include<math.h>
int main()
{
    int num,ld,digit,sum,i,end;
    scanf("%d",&end);
    for(i=1;i<=end;i++)
    {
        sum=0;
        num=i;
        digit=(int)log10(num);
        while(num>0)
        {
            ld=num%10;
            sum+=ceil(pow(ld,digit));
            num=num/10;
        }
        if(i==sum)
          {
             printf("%d is a Armstrong number\n",i);
             printf("153 is a Armstrong number\n");
          }
    }      
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/c2bec4f0-9ef0-4824-947d-5bff12cedc6e)
## RESULT:
Thus, C Program to print Armstrong Numbers between 1 to n has successfully executed.

# EX3(C)-ARRAYS
## AIM:
Write a program in C to read n number of values in an array and display it in reverse order
## ALGORITHM:
Step 1: Include the necessary header file stdio.h.

Step 2: Declare integer variables n and arr[10], and a loop counter variable i.

Step 3: Read an integer input for n from the user.

Step 4: Start a loop to input n elements into the arr array.

    Initialize i to 0.
    Read integers and store them in arr[i].

Step 5: Start another loop to print the elements in reverse order.
    
Step 6: Initialize i to n-1.

Step 7: Print arr[i] followed by a space.

Step 8: The program terminates once all elements are printed in reverse order.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int n,arr[10],i;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    for(i=n-1;i>=0;i--)
    {
        printf("%d ",arr[i]);   
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/ee542aa2-147a-4050-a78b-84c9f53b12a7)
## RESULT:
Thus,the C program executed successfully.

# EXP3(D)-ARRAYS-AND-ITS-TYPES
## AIM:
Write a C program to search an element in an array 
## ALGORITHM:
Step 1: Include the necessary header file stdio.h.

Step 2: Declare integer variables n, i, and x, and an integer array arr[20].

Step 3: Read an integer input for n from the user.

Step 4: Start a loop to input n elements into the arr array.

    Initialize i to 0.
Step 5: Read integers and store them in arr[i].

Step 6: Set the value of x to 5, the value to be searched for in the array.

Step 7: Start a loop to search for the value x in the array.

    Initialize i to 0.
Step 8: Check if arr[i] is equal to x.

Step 9: If true, print that x is found at position x.

Step 10: The program terminates once the second loop completes its search.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int n,i,x;
    scanf("%d",&n);
    int arr[20];
    for(i=0;i<n;i++)
    {
        scanf("%d ",&arr[i]);
    }
    x=5;
    for(i=0;i<n;i++)
    {
        if(arr[i]==x)
        {
            printf("%d is found at position %d",x,x);
        }  
    }   
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/63281daa-fd90-4fff-a679-222158ee96ad)
## RESULT:
Thus,  C program to search an element in an array  is successfully executed.

# EX4(A)-DATATYPES AND OPERATORS
## AIM:
To write a Program to check whether a given character is upper case, lower case, number or special character using conditional operator
## ALGORITHM:
1. Include the <stdio.h> header file.

2. Define the main function.

3. Declare a character variable named let.

4. Read a character from the user using scanf.

5. Check the character's category using if-else statements based on ASCII values.

6. If the character is uppercase (ASCII 65-90), print "Upper."

7. If the character is lowercase (ASCII 97-122), print "Lower."

8. If the character is a number (ASCII 48-57), print "Number."

9. If the character doesn't fall into the above categories, print "Symbol."
## PROGRAM:
~~~
#include <stdio.h>
int main()
{
   char let;
    scanf("%c",&let);

   if(let>=65 && let<=90)
     {
       printf("Upper");
     }
   else if(let>=97 && let<=122)
    {
       printf("Lower");
    }
    else if(let>=48 &&let<=57)
   {
      printf("Number");
}
    else
       {
          printf("Symbol");
}
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/22a1cb3c-c981-4081-a25b-336d753d62f2)
## RESULT:
Thus, the c program executed successfully

# EX4(B)-UNCONDITIONAL STATEMENTS
## AIM:
To write a C Program to check whether the given triangle is isosceles, equilateral, or scalene triangles using an if-else ladder.
## ALGORITHM:
1.Include the <stdio.h> header file.

2.Define the main function.

3.Declare three integer variables: a, b, and c.

4.Read three integers from the user using scanf.

5.Check if all three sides are equal (Equilateral) using if condition with a == b && a == c.

6.If not all sides are equal, check if at least two sides are equal (Isosceles) using else if with (a == b && a != c) || (a != b && a == c).

7.If none of the above conditions are met, it's a Scalene triangle.

8.Print the corresponding triangle type based on the condition met.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int a,b,c;
    scanf("%d %d %d ",&a,&b,&c);
    if(a==b && a==c)
    {
        printf("Equilateral triangle.");
    }
    else if((a==b && a!=c) || (a!=b && a==c))
    {
        printf("Isosceles triangle.");
    }
    else
    {
        printf("Scalene triangle.");
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/b872846d-29cf-4109-a139-aa3152049725)
## RESULT:
Thus, program to check the triangle has been executed successfully.

# EX4(C)-STRINGS
## AIM:
To find the length of the given string.
## ALGORITHM:
1. Include the necessary header files: <stdio.h> and <string.h>.

2. Define the main function.

3. Declare a character array Str with a size of 10 to store a string.

4. Declare an integer variable i for counting characters in the string.

5. Read a string from the user using scanf.

6. Use a for loop to iterate through the characters in the string until the null character '\0' is encountered.

7. Inside the loop, increment the i variable for each character.

8. After the loop, print the length of the string using printf.
## PROGRAM:
~~~
#include <stdio.h>
#include <string.h>
  
 int main()
{
    char Str[10];
    int i;
    scanf("%s", Str);
    for (i = 0; Str[i] != '\0'; ++i)
    {
        
    }
    printf("Length of Str is %d",i );
  return 0;  
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/1124e053-2b61-4203-ae4a-3fb31baca324)
## RESULT:
Thus, program To find the length of the given string has executed successfully.

# EX4(D)-STRING APPLICATION
## AIM:
To Write a C program to reverse a string using loops
## ALGORITHM:
1. Include the necessary header files: <stdio.h> and <string.h>.

2. Define the main function.

3. Declare a character array str with a size of 20 to store a string.

4. Read a line of text (including spaces) from the user until the newline character is encountered using scanf with the format specifier %[^\n].

5. Print the entered string using printf.

6. Print "Reversed string is: " to indicate the reversed string.

7. Use a for loop to iterate in reverse order through the characters of the string, starting from the last character (determined by strlen(str) - 1) down to the first character (index 0).

8. Inside the loop, print each character in reverse order.
## PROGRAM:
~~~
#include<stdio.h>
#include<string.h>


int main()
{
    char str[20];
    scanf("%[^\n]",str);
    printf("Entered string is: %s\n",str);
    printf("Reversed string is: ");
    for(int i=(strlen(str)-1);i>=0;i--)
    {
         printf("%c",str[i]);
    }
    return 0;
    //printf("Reversed string is: %s",str(str));
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/ab7d56a4-ee00-4498-ac3c-a0a6939d30b2)
## RESULT:
Thus,program to reverse a string using loops has executed successfully.

# EX5(A)-POINTERS
## AIM:
To Write a C program to test whether the number is equal to zero or not by using pointers. 
## ALGORITHM:
1. Include the <stdio.h> header file.

2. Define the main function.

3. Declare an integer variable a to store an integer.

4. Declare an integer pointer p.

5. Read an integer from the user and store it in variable a using scanf.

6. Point the pointer p to the address of the variable a.

7. Check the value pointed to by p:

    If it's greater than 0, print "the number is Positive."
    If it's less than 0, print "the number is Negative."
    If it's equal to 0, print "the number is equal to zero."
8.End the program.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    int a;
    int *p;
    scanf("%d",&a);
    p=&a;
    if(*p > 0)
    {
        printf("the number is Positive");
    }
    else if(*p<0)
    {
        printf("the number is Negative");
    }
    else if (*p == 0)
    {
        printf("the number is equal to zero");
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/ec8f6119-bacd-478e-8bd2-1b5ec785091a)
## RESULT:
Thus, C program to test whether the number is equal to zero or not by using pointers has executed successfully.

# EX5(B)-FUNCTIONS AND STORAGE CLASS
## AIM:
To Write a C program to calculate the GCD of 144,270 using Recursion.
## ALGORITHM:
1. Include the <stdio.h> header file.

2.Define the gcd function that takes two integers, a and b, as parameters.

    If b is equal to 0, return a as the GCD (base case).
    Otherwise, recursively call the gcd function with arguments b and a % b.
3. Define the main function.

4. Declare two integer variables, num1 and num2, and an integer variable result.

5. Set the values of num1 and num2 to 144 and 270, respectively.

6. Swap the values of num1 and num2 if num1 is less than num2 to ensure num1 is greater or equal to num2.

7. Calculate the GCD of num1 and num2 using the gcd function and store the result in the result variable.

8. Print the result, indicating the GCD of num2 and num1.
## PROGRAM:
~~~
#include <stdio.h>
int gcd(int a, int b) {
    if (b == 0) {
        return a; // Base case: GCD is found when b becomes 0
    } else {
        return gcd(b, a % b); // Recursive case: GCD calculation
    }
}
int main() {
    int num1 = 144;
    int num2 = 270;
    int result;

    // Ensure num1 is greater than or equal to num2 for the algorithm to work correctly
    if (num1 < num2) {
        int temp = num1;
        num1 = num2;
        num2 = temp;
    }
    result = gcd(num1, num2);
    printf("G.C.D of %d and %d is %d.\n", num2, num1, result);
    return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/586521c6-490f-4c8a-83e6-8091d47caa98)
## RESULT:
Thus, C program to calculate the GCD of 144,270 using Recursion has successfully executed.

# EXP5(C)-ARRAYS AND ITS OPERATIONS
## AIM:
To Write a C Program to print the Opposite Diagonal Elements of a Matrix[3x3]
## ALGORITHM:
1.Include the <stdio.h> header file.

2. Define the main function.

3. Declare integer variables m, n, i, and j.

4. Read two integers, m and n, from the user, representing the dimensions of the matrix.

5. Declare a 2D integer array arr with dimensions m rows and n columns.

6. Use nested loops to read m rows and n columns of integer values into the arr matrix.

7. Print the message "The Diagonal Elements of a Matrix = " to indicate the output.

8. Use a loop to iterate through the diagonal elements of the matrix and print them.

   Initialize i to 0 and j to m - 1.
   While i is less than n and j is greater than or equal to 0, print the value of arr[i][j].
   Increment i and decrement j in each iteration.

## PROGRAM:
~~~
#include <stdio.h>

int main()
{
     int m,n,i,j;
     scanf("%d %d",&m,&n);
    int arr[m][n];
    for(i=0;i<m;i++)
{
     for(j=0;j<m;j++)
{
      scanf("%d ",&arr[i][j]);
}
}
printf("The Diagonal Elements of a Matrix = ");
for(i=0,j=m-1; i<n && j>=0;i++,j--)
{
printf("%d ",arr[i][j]);
}
return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/bf95b18e-3f8c-427b-bde3-d819021641b2)
## RESULT:
 Thus,C Program to print the Opposite Diagonal Elements of a Matrix[3x3] has executed successfully.

 # EX5(D)-STRINGS
 ## AIM:
To Write a program in C to print all the alphabets using pointer.
## ALGORITHM:
1. Include the <stdio.h> header file.

2. Define the main function.

3. Declare a character array str of size 50 and initialize it with the string "ABCDEFGHIJKLMNOPQRSTUVWXYZ."

4. Declare a character pointer p to store the address of the string.

5. Initialize an integer variable i to 0.

6. Print the message "The Alphabets are:" to indicate the output.

7. Use a while loop to iterate through the string str until the null character '\0' is encountered.

    Inside the loop, print the character pointed to by p, increment the pointer p, and increment i.

8. End the program.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
    char str[50]="ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    char *p;
    p=str;
    int i=0;
    printf("The Alphabets are : \n");
    while(str[i]!='\0')
    {
       printf(" %c ",*p); 
       p++;
       i++;
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/9be2d40b-0103-4c9b-8a51-7d9bea9a3354)
![image](https://github.com/vidhyadharan-03/c/assets/114286357/94c43f36-1109-4fc6-8c84-244debb98601)
## RESULT:
Thus, program in C to print all the alphabets using pointer has successfully executed.

# EX6(A)-POINTERS
## AIM:
To write a c program to find sum and average in the range from 30 to 35 using pointer.
## ALGORITHM:
1. Include the <stdio.h> header file.

2.Define the main function.

3. Declare integer variables m, n, and i.

4. Declare integer pointers pm and pn, and double variables sum and avg.

5. Declare double pointers psum and pavg and assign the addresses of sum and avg to them.

6. Read two integers m and n from the user using scanf.

7. Use a for loop to calculate the sum of integers from m to n and store it in sum.

8. Calculate the average avg using the formula: avg = sum / (n - m + 1).

9. Print the sum and average values with two decimal places using printf.

10. End the program with a return 0; statement.
## PROGRAM:
~~~
#include<stdio.h>
int main()
{
  int m, n, i;
  int *pm, *pn;
  pm= &m, pn= &n;
  double sum=0.0, avg;
  double *psum, *pavg;
  psum= &sum, pavg= &avg;
  scanf("%d %d", pm, pn);
  for(i=m;i<=n;i++)
  {
    *psum += i;
  }
  *pavg= (*psum) / (*pn - *pm + 1);
  printf("Sum= %.2lf, Average= %.2lf", *psum, *pavg);
  return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/d6663d19-2fe2-4a88-bd06-f211334f949e)
## RESULT:
Thus, c program to find sum and average in the range from 30 to 35 using pointer has successfully executed.

# EX6(B)-DYNAMIC MEMORY ALLOCATION
## AIM:
To Write a C program to check given input is even or odd using calloc()
## ALGORITHM:
1. Include the <stdio.h> and <stdlib.h> header files.

2. Define the main function.

3. Declare an integer variable a to store an integer input.

4. Read an integer from the user and store it in the variable a using scanf.

Allocate memory for an integer pointer p using calloc, which is unnecessary in this code as you directly assign the address of a to p.

5. Assign the address of the variable a to the pointer p.

6. Check if the value pointed to by p is even or odd.

7. If it's even, print "a is Even Number" with the value of a.

8. If it's odd, print "a is Odd Number" with the value of a.

9. End the program with a return 0; statement.
## PROGRAM:
~~~
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int a;
    scanf("%d",&a);

    int *p =(int *)calloc(1,sizeof(int));
    p=&a;
    if(*p%2==0)
    {
        printf("%d is Even Number",*p);
    }
    else
    {
        printf("%d is Odd Number",*p);
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/cf854eef-6126-4f92-a598-4f74ecbf96c2)
## RESULT:
C program to check given input is even or odd using calloc() has successfully executed.

# EX6(C)-STRUCTURE
## AIM:
Create a C program to store the information of 5 students by using an array of structures.
## ALGORITHM:
1. Include the <stdio.h> header file.

2. Define a structure named students with members name (a character array) and marks (a floating-point number).

3. Declare an array of students named S with a size of 5.

4. Define the main function.

5. Use a for loop to read student information for 5 students, including their names and marks, and store it in the S array.

6. Print the message "Displaying Information:" to indicate the output.

7. Use another for loop to display the information for each student, including the roll number (indexed from 1), name, and marks.

8. End the program.
## PROGRAM:
~~~
#include<stdio.h>
struct students
{
   //int rollno;
   char name[20];
   float marks;
}S[5];
int main()
{
   int i;
   for(i=0;i<5;i++)
    {
       scanf("%s %f",S[i].name,&S[i].marks);
    }
printf("Displaying Information:\n");
    for(i=0;i<5;i++)
    {
         
         printf("Roll number: %d\nFirst name: %s\nMarks: %.1f\n\n",
                 i+1,S[i].name,S[i].marks);
    }
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/ee190db5-6187-4987-b35d-f79416afadf8)
## RESULT:
Thus, C program to store the information of 5 students by using an array of structures has successfully executed.

# EX6(D)-USER DEFINED DATA-TYPES
## AIM:
write a program to display the class timings using enumeration (like first hour=8 am...fifth hour=12 pm)
## ALGORITHM:
1. Include the <stdio.h> header file.

2. Define an enumeration named ClassHours to represent class hours, starting from 8 am.

3. Define the main function.

4. Print "Class Timings" to indicate the output.

5. Use the enumeration constants to display class timings for each hour, both in the morning (am) and in the afternoon (pm).

6. End the program with a return 0; statement.
## PROGRAM:
~~~
#include <stdio.h>

// Enumeration for class hours
enum ClassHours {
    FIRST_HOUR = 8,
    SECOND_HOUR,
    THIRD_HOUR,
    FOURTH_HOUR,
    FIFTH_HOUR
};

int main() {
    printf("Class Timings\n");
    
    // Display class timings using the enumeration
    printf("First Hour = %d am\n", FIRST_HOUR);
    printf("second Hour = %d am\n", SECOND_HOUR);
    printf("Third Hour = %d am\n", THIRD_HOUR);
    printf("Fourth Hour = %d am\n", FOURTH_HOUR);
    printf("Fifth Hour = %d pm\n", FIFTH_HOUR);

    return 0;
}
~~~
## OUTPUT:
![image](https://github.com/vidhyadharan-03/c/assets/114286357/9a3947de-887e-4d6c-9744-7186fff746a7)
## RESULT:
 program to display the class timings using enumeration (like first hour=8 am...fifth hour=12 pm) has successfully executed.




