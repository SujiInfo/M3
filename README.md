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
   #include <stdio.h>
   #include <math.h>
   
   void cemi(float p, float r, float n) {
       float emi;
       r = r / (12 * 100); /* one month interest */
       n = n * 12;        /* total months */
       emi = (p * r * pow(1 + r, n)) / (pow(1 + r, n) - 1);
       printf("Monthly EMI is= %.3f\n", emi);
   }
   
   int main() {
       float principal, rate, time;
       printf("Enter principal, rate, and time: ");
       scanf("%f %f %f", &principal, &rate, &time);
       cemi(principal, rate, time);
       return 0;
   }

## OUTPUT

![image](https://github.com/user-attachments/assets/9b4e0ba2-d9b7-4d09-b4cf-f4f458db7b6b)





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

   #include <stdio.h>
   
   int main() {
       int n = 6;
       int a = 0, b = 1, next;
   
       printf("Fibonacci Series for %d terms:\n", n);
       printf("%d, %d", a, b);
   
       for (int i = 3; i <= n; i++) {
           next = a + b;
           printf(", %d", next);
           a = b;
           b = next;
       }
       printf("\n");
       return 0;
   }


## OUTPUT


![image](https://github.com/user-attachments/assets/8a67f6e8-3d29-4ef5-84df-dc44574e3ada)







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
       printf("The last element of the array is: %d\n", arr[n - 1]);
       return 0;
   }

## OUTPUT


![image](https://github.com/user-attachments/assets/7e576029-65b4-43a8-bf92-a12ef911d4c1)








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
  #include <stdio.h>
  
  int main() {
      int n, c = 0;
      scanf("%d", &n);
      int a[n];
      for (int i = 0; i < n; i++) {
          scanf("%d", &a[i]);
          if (a[i] > 0) {
              c++;
          }
      }
      printf("count of positive numbers in array: %d\n", c);
      return 0;
  }

## OUTPUT

![image](https://github.com/user-attachments/assets/c67bbea3-f1ee-41b4-b042-e7742dc7ca20)





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
  #include <stdio.h>
  
  int main() {
      int n;
      printf("Enter Number of elements: ");
      scanf("%d", &n);
      char arr[n];
      printf("Enter elements: ");
      for (int i = 0; i < n; i++) {
          scanf(" %c", &arr[i]);
          if ((int)arr[i] % 2 == 0) arr[i] = 'E';
      }
      for (int i = 0; i < n; i++) {
          if (arr[i] == 'E') {
              printf("E ");
          } else {
              printf("%c ", arr[i]);
          }
      }
      printf("\n");
      return 0;
  }
## Output:

 ![image](https://github.com/user-attachments/assets/567daba7-a66a-4ef8-896b-de128955c982)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



