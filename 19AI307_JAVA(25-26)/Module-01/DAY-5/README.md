# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to count the frequency of a given character in a string.

Input	Result
scanner
n
Frequency of 'n' is: 2


## AIM:
To write a Java program that reads a string and a character from the user and calculates how many times the given character appears in the string.

## ALGORITHM :
1. Start the program and create a Scanner object to read user input.

2. Read a full string from the user.

3. Read a single character whose frequency needs to be counted.

4. Initialize a counter variable to zero.

5. Loop through each character of the string.

6. Check if the current character matches the given character; if yes, increment the counter.

7. After the loop ends, display the total frequency of the character.



## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        String str = sc.nextLine();
        char ch = sc.nextLine().charAt(0);
        int count = 0;
        for(int i = 0; i < str.length(); i++){
            if(str.charAt(i) == ch) count++;
        }
        System.out.println("Frequency of '" + ch + "' is: " + count);
    }
}
```




## OUTPUT:
<img width="637" height="370" alt="image" src="https://github.com/user-attachments/assets/f9408ce9-ae78-4dd9-9c1a-f847068925d0" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.
