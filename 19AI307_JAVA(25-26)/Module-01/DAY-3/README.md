# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
A left-aligned triangle pattern is a pattern of stars (*) where each row contains an increasing number of stars, aligned to the left side.

Write a Java program that:

Prompts the user to enter the number of rows for the triangle.

Uses nested loops to print the left-aligned triangle pattern.

Ensures that each row contains stars corresponding to its row number.

For example:

Input	Result
3
* 
* * 
* * * 


## AIM:
To write a Java program that prints a left-aligned right-angled triangle pattern using asterisks based on the number of rows entered by the user.

## ALGORITHM :
1. Start the program and create a Scanner object to read input from the user.


2. Read an integer value representing the number of rows for the triangle.


3. Use an outer loop to iterate from 1 to the given number of rows.


4. Use an inner loop to print asterisks equal to the current row number.


5. After printing each row, move to the next line.


6. Continue the process until the full triangle pattern is displayed.



## PROGRAM:
 ```
/*Program to implement a Looping concept using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
public class LeftAlignedTriangle {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int rows = scanner.nextInt();
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```



## OUTPUT:
<img width="374" height="502" alt="image" src="https://github.com/user-attachments/assets/efb49299-19e5-4f1e-9ceb-1005892ac950" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.

