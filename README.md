## EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:

#include <stdio.h>
int main() 
{
    char firstChar, secondChar, thirdChar;
    scanf(" %c", &firstChar);
    scanf(" %c", &secondChar);
    scanf(" %c", &thirdChar);
    printf("%c %c %c\n", thirdChar, secondChar, firstChar);
    return 0;
}

## OUTPUT:



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

#include <stdio.h>
int main() 
{
    int a;
    scanf("%d", &a);
    if (a > 0) {
        printf("Positive number\n");
    } else {
        printf("Not a positive number\n");
    }
    return 0;
}

# OUTPUT:

<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/e8c4b016-67a8-487c-b25b-a57101172b58" />


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

#include <stdio.h>
int main() {
    int num1, denom1, num2, denom2;
    float fraction1, fraction2, minFraction;
    printf("Enter numerator and denominator for first fraction: ");
    scanf("%d %d", &num1, &denom1);
    printf("Enter numerator and denominator for second fraction: ");
    scanf("%d %d", &num2, &denom2);
    fraction1 = (float) num1 / denom1;
    fraction2 = (float) num2 / denom2;
    printf("Fraction 1: %d/%d = %.4f\n", num1, denom1, fraction1);
    printf("Fraction 2: %d/%d = %.4f\n", num2, denom2, fraction2);
    minFraction = (fraction1 < fraction2) ? fraction1 : fraction2;
    printf("Minimum fraction value: %.4f\n", minFraction);
    return 0;
}


## OUTPUT:

<img width="1920" height="1080" alt="Screenshot (48)" src="https://github.com/user-attachments/assets/e8db3cc1-675b-4ffa-895c-5bfbdd8ce651" />


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

#include <stdio.h>
int main() 
{
    int inputValue;
    scanf("%d", &inputValue);
    if (inputValue == 1) {
        printf("Input is equal to 1\n");
    } else {
        printf("Input is not equal to 1\n");
    }
    return 0;
}

## OUTPUT:

<img width="1920" height="1080" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/53a77ef2-0f7f-40f0-a477-21b937c22ee3" />


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

#include <stdio.h>
int main()
 {
    int mark1, mark2, mark3;
    float total, percentage;
    scanf("%d", &mark1);
    scanf("%d", &mark2);
    scanf("%d", &mark3);
    total = mark1 + mark2 + mark3;
    percentage = total / 3;
    printf("%.2f\n", total);
    printf("%.2f\n", percentage);
    if (mark1 >= 40 && mark2 >= 40 && mark3 >= 40) {
        if (percentage >= 60) {
            printf("Division = First\n");
        } else if (percentage >= 48) {
            printf("Division = Second\n");
        } else if (percentage >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    } else {
        printf("Division = Fail\n");
    }
    return 0;
}

## OUTPUT:

<img width="1920" height="1080" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/9527f76d-cd27-4a01-b00f-47d0c310462d" />


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

