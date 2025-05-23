# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
~~~
#include <stdio.h>
#include <math.h>

void calculateEMI(float p, float R, int T);

int main() {
    float p, R;
    int T;
    printf("Enter loan amount : ");
    scanf("%f", &p);
    printf("Enter interest rate : ");
    scanf("%f", &R);
    printf("Enter tenure: ");
    scanf("%d", &T);
    calculateEMI(p, R, T);
    return 0;
}

void calculateEMI(float p, float R, int T) {
    float monthlyRate = R / (12 * 100); 
    int tenureMonths = T * 12;
    float emi;

    emi = (p * monthlyRate * pow(1 + monthlyRate, tenureMonths)) /
          (pow(1 + monthlyRate, tenureMonths) - 1);

    printf("\nYour EMI is: ₹%.2f per month\n", emi);
}
~~~

## OUTPUT

![image](https://github.com/user-attachments/assets/26a1dcdd-a041-4701-bee6-5d1fdbeade88)




## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
~~~
#include <stdio.h>
int main() {
    int n ; scanf("%d",&n);  
    int first = 0, second = 1, next;
    printf("Fibonacci series for %d terms:\n", n);
    for (int i = 0; i < n; i++) {
        if (i <= 1)
            next = i;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }
    printf("\n");
    return 0;
}
~~~
## OUTPUT

![image](https://github.com/user-attachments/assets/200553f8-6b6e-4701-a641-9c5c7584aeb8)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
~~~`
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}
~~~
## OUTPUT


![image](https://github.com/user-attachments/assets/1d409f01-bd81-41e3-96d3-e67be14da729)







## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
~~~
#include <stdio.h>
int main() {
    int n, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);

    return 0;
}
~~~

## OUTPUT


![image](https://github.com/user-attachments/assets/6f460fec-0a47-460f-9328-7d964c80b2f0)



## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
~~~
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d integers:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Modified array :\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}
~~~
## Output:
 
![image](https://github.com/user-attachments/assets/e216d54e-dd58-434b-91ad-586e887a3dbd)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



