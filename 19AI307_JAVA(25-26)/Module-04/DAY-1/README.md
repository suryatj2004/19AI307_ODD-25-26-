# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:

You are reading multiple strings from the user and want to print their lengths. Sometimes the input might be null. What exception could occur if you try to get the length of a null string? How would you handle it gracefully in your code?


## AIM:
To write a Java program that reads strings continuously and handles null input using exception handling.

## ALGORITHM :
1. Create a Scanner object to read input from the user.

2. Use a loop to read each line until no more input exists.

3. Check if the string is "null" or actually null.

4. If so, throw a NullPointerException.

5. Catch the exception and print "Null string encountered".

6. Otherwise, print the length of the input string.

7. Continue until all inputs are processed.

8. Close the Scanner.




## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        while (sc.hasNextLine()) {
            String str = sc.nextLine();
            try {
                if (str == null || str.equals("null"))
                    throw new NullPointerException();
                System.out.println("Length: " + str.length());
            } catch (NullPointerException e) {
                System.out.println("Null string encountered");
            }
        }
        sc.close();
    }
}

```




## OUTPUT:

<img width="685" height="293" alt="image" src="https://github.com/user-attachments/assets/a3e53432-e642-42db-a977-1e2b11cf85d8" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
