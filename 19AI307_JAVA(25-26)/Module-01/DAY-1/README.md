# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:

Lovely is now a potion apprentice at the Wizardry Academy. Every potion has to be made by mixing ingredients of different data types like int, double, byte, and float.

However, the mixing cauldron accepts only one type at a time, so she has to type cast the ingredients to prepare the final mix.

Lovely experiments with explicit and implicit type casting to see how different types behave when converted into others.

Task:
Read four types of values:

An int

A double

A float

A byte

Perform the following conversions:

Convert the int to double (implicit)

Convert the double to int (explicit)

Convert the float to int (explicit)

Convert the byte to float (implicit)

Print the results of each conversion.

Input Format:
First line: Integer value

Second line: Double value

Third line: Float value

Fourth line: Byte value

Output Format:

Int to Double: <value>
Double to Int: <value>
Float to Int: <value>
Byte to Float: <value>

For example:

Input	Result
42
99.99
78.5
5
Int to Double: 42.0
Double to Int: 99
Float to Int: 78
Byte to Float: 5.0

## AIM:
To write a Java program that demonstrates type conversion between different primitive data types, including widening and narrowing conversions, and to display the results of each conversion.

## ALGORITHM :
1. Start the program and create a Scanner object to read inputs from the user.

2. Read an integer, a double, a float, and a byte value from the user.

3. Convert the integer to a double (widening conversion) and store the result.

4. Convert the double to an integer (narrowing conversion) and store the result.

5. Convert the float to an integer (narrowing conversion) and store the result.

6. Convert the byte to a float (widening conversion) and store the result.

7. Display all the converted results to the user.



## PROGRAM:
```
/*
Program to implement variables and Operators using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## Sourcecode.java:
```
import java.util.*;
public class main{
    public static void main(String[]args){
        Scanner scan=new Scanner(System.in);
        int a=scan.nextInt();
        double b=scan.nextDouble();
        float c=scan.nextFloat();
        byte d=scan.nextByte();
        double res1=a;
        int res2=(int)b;
        int res3=(int)c;
        float res4=d;
        System.out.println("Int to Double: "+res1);
        System.out.println("Double to Int: "+res2);
                System.out.println("Float to Int: "+res3);
                        System.out.println("Byte to Float: "+res4);
    }
}
```
## OUTPUT:

<img width="558" height="612" alt="image" src="https://github.com/user-attachments/assets/e202beae-bb90-4e01-a39c-7f11d1c269ef" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
