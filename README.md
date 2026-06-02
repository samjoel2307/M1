# EX-01-Datatypes-Operators

## NAME:B.SAM JOEL JOSHUA

## REGISTER NO: 212225230242

## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    char ch1,ch2,ch3;
    scanf("%c %c %c",&ch1,&ch2,&ch3);
    printf("The reverse of %c%c%c is %c%c%c",ch1,ch2,ch3,ch3,ch2,ch1);
    return 0;
}
```
## OUTPUT:

<img width="906" height="167" alt="Screenshot 2026-03-25 090427" src="https://github.com/user-attachments/assets/8f757f4a-5510-4b47-b43d-dc0dcaba7ee8" />

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    if(num>0)
    {
        printf("%d is Positive",num);
    }
    else if(num<0)
    {
        printf("%d is Negative",num);
    }
    else
    {
        printf("0");
    }
    return 0;
}
```
# OUTPUT:

<img width="902" height="167" alt="Screenshot 2026-03-25 090621" src="https://github.com/user-attachments/assets/69bdf594-4cbf-40df-91cd-0491014742bf" />

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    float n1,d1,n2,d2,min;
    printf("Enter the numerator and denominator:");
    scanf("%f %f %f %f",&n1,&d1,&n2,&d2);
    min=(n1/d1<n2/d2)?n1/d1:n2/d2;
    printf("The minimum value is %f",min);
    return 0;
}
```
## OUTPUT:

<img width="908" height="250" alt="Screenshot 2026-03-25 090908" src="https://github.com/user-attachments/assets/296a7246-66db-454a-98f3-2dbf8c3f78e5" />


## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.


# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    if(num==1)
    {
        printf("Number is equal to 1");
    }
    else
    {
        printf("Number is not equal to 1");
    }
    return 0;
}
```
## OUTPUT:

<img width="903" height="165" alt="Screenshot 2026-03-25 091106" src="https://github.com/user-attachments/assets/3e878072-2ad8-4dd9-9266-b5bf5a68b7af" />

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully


# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m1,m2,m3;
    float total,per;
    scanf("%d %d %d",&m1,&m2,&m3);
    total=m1+m2+m3;
    per=100*(total/300);
    printf("Total marks = %f\n",total);
    printf("Percentage = %f\n",per);
    if(m1>=40&&m2>=40&&m3>=40)
    {
        if(per>=60)
        {
            printf("Division = First");
        }
        else if(per>=48)
        {
            printf("Divison = Second");
        }
        else if(per>=36)
        {
            printf("Division = Pass");
        }
    }
    else
    {
        printf("Division = Fail");
    }
    return 0;
}
```

## OUTPUT:

<img width="906" height="282" alt="Screenshot 2026-03-25 091306" src="https://github.com/user-attachments/assets/0cffe92c-993a-4486-8071-2d0bf2850c72" />

<img width="910" height="274" alt="Screenshot 2026-03-25 091415" src="https://github.com/user-attachments/assets/c9eb3372-a3b2-4bbf-bba5-f75e9012bfe3" />

<img width="912" height="277" alt="Screenshot 2026-03-25 091606" src="https://github.com/user-attachments/assets/1bfacbf8-5a70-49dd-b03b-9cc7a2e0c6ca" />

<img width="910" height="276" alt="Screenshot 2026-03-25 091713" src="https://github.com/user-attachments/assets/b4af5f5c-9a50-4786-bdc8-ccfdbe6b4ad9" />


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.
