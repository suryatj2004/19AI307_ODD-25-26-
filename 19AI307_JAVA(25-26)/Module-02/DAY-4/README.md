# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a java program using class to perform addition of two numbers using parameterised constructor.

Input	Result
5
5
Sum = 10

## AIM:
To write a Java program that demonstrates the use of constructors by creating a class that adds two numbers using a parameterized constructor and displays the result.

## ALGORITHM :
1. Define a class Add with an integer variable sum.

2. Create a parameterized constructor that accepts two integers and stores their addition in sum.

3. Define a method display() to print the calculated sum.

4. In the main method, create a Scanner object to read two integers from the user.

5. Read the two integer inputs and store them in variables.

6. Create an object of the Add class, passing the two numbers to the constructor.

7. Call the display() method to show the result.

8. End the program.





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.Scanner;
class Add {
    int sum;
    Add(int a, int b) {
        sum = a + b;
    }
    void display() {
        System.out.println("Sum = " + sum);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num1 = sc.nextInt();
        int num2 = sc.nextInt();
        Add obj = new Add(num1, num2);
        obj.display();
    }
}
```





## OUTPUT:
<img width="399" height="369" alt="image" src="https://github.com/user-attachments/assets/5b14a4a6-8a03-45e1-a08a-0653983ec277" />



## RESULT:

The program has been executed successfully and the desired output has been obtained.
