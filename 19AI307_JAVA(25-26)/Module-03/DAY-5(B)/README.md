# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to check if a number is an Armstrong number using Math.pow() and the Integer wrapper class. Take input from the user.

Input	Result
153
153 is an Armstrong number.


## AIM:
To write a Java program to check whether a given number is an Armstrong number.

## ALGORITHM :

1. Read a number from the user.

2. Convert the number to a string to find the number of digits.

3. Initialize sum = 0 and copy the number to a temporary variable.

4. Extract each digit using modulus.

5. Raise each digit to the power of the total digits and add it to sum.

6. After the loop, compare sum with the original number.

7. If both are equal, print Armstrong number; otherwise print not Armstrong.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ArmstrongChecker {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int number = sc.nextInt();
        String numStr = Integer.toString(number);
        int length = numStr.length();

        int sum = 0;
        int temp = number;

        while (temp != 0) {
            int digit = temp % 10; // get last digit
            sum += (int) Math.pow(digit, length);
            temp /= 10; // remove last digit
        }

        if (sum == number) {
            System.out.println(number + " is an Armstrong number.");
        } else {
            System.out.println(number + " is not an Armstrong number.");
        }
    }
}

```

## OUTPUT:

<img width="776" height="336" alt="image" src="https://github.com/user-attachments/assets/a9fcac73-2b8a-425c-8e9e-a258be0eb0fe" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
