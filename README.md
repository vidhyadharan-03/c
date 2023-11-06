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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/0f97087a-245e-4770-9148-182abd47488f)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/736393e1-0a03-46e7-8e9c-86ebbbdf53e6)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/8ddab278-32a1-404e-9ccf-b1a3e349fa2b)

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

![image](https://github.com/vidhyadharan-03/c/assets/114286357/e59ccebf-e722-4965-9b8c-7bce34a6c09b)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/dff9b5c6-2e80-4e1f-b602-ca0664c706b7)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/26f09f67-603e-49d2-86b2-8ce3e302edcb)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/46c2f314-1463-466b-950f-6ca07d949edc)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/fe31a4fe-853d-43de-a387-c2ee910a3a49)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/e459602b-e78c-431d-a962-a59416a8c4bd)

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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/594afae2-6481-4cdb-9af2-497f35c8b465)
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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/fcefcb1e-1719-44bf-99c6-e22d671a389f)
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
![image](https://github.com/vidhyadharan-03/c/assets/114286357/f5a014eb-7964-44b8-a247-a208c09b2cd0)
## RESULT:
Thus,  C program to search an element in an array  is successfully executed.

# 








