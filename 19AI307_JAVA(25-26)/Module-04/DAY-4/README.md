# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
You need to clone documents. Implement the Prototype Pattern to copy a Document object with a title and content. On user input, create a copy and print both the original and the clone.

For example:

Input	Result
Resume
Experienced Java Developer
Original: Resume - Experienced Java Developer
Cloned: Resume - Experienced Java Developer


## AIM:
To write a Java program that demonstrates object cloning by creating a Document object and producing its copy using the clone() method.

## ALGORITHM :
1. Create a class Document that implements Cloneable.

2. Define variables for title and content and initialize them using a constructor.

3. Override the clone() method to return a copy of the object.

4. In main(), read the title and content from the user.

5. Create an original Document object using the input.

6. Clone the original document using the clone() method.

7. Print both the original and cloned document details.





## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.*;
class Document implements Cloneable {
    String title;
    String content;
    Document(String title, String content) {
        this.title = title;
        this.content = content;
    }
    public Document clone() {
        try {
            return (Document) super.clone();
        } catch (CloneNotSupportedException e) {
            return null;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String title = sc.nextLine();
        String content = sc.nextLine();
        Document original = new Document(title, content);
        Document clone = original.clone();
        System.out.println("Original: " + original.title + " - " + original.content);
        System.out.println("Cloned: " + clone.title + " - " + clone.content);
        sc.close();
    }
}

```




## OUTPUT:
<img width="1231" height="369" alt="image" src="https://github.com/user-attachments/assets/82a7d527-a64f-46fb-aa19-71cbb1587234" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.
