# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Counter with a static integer variable count. Every time an object is created, increase count by 1. Print the total count using a static method


class Counter {
    static int count = 0;
     // Your Code Here
}

class prog {
    public static void main(String[] args) {
        // Your Code Here
    }
}

 

For example:

Result
Total objects created: 7


## AIM:
To write a Java program that demonstrates the use of static variables and static methods by counting the number of objects created using a Counter class and displaying the total count.

## ALGORITHM :
1. Define a class Counter with a static integer variable count initialized to 0.

2. Create a constructor that increments the static variable count each time a new object is created.

3. Define a static method displayCount() that prints the total number of objects created.

4. In the main method, create multiple objects of the Counter class.

5. After creating the objects, call the static method Counter.displayCount() to display the final count.

6. End the program.




## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
class Counter {
    static int count = 0;
    Counter() {
        count++;
    }
    static void displayCount() {
        System.out.println("Total objects created: " + count);
    }
}
class prog {
    public static void main(String[] args) {
        new Counter();
        new Counter();
        new Counter();
        new Counter();
        new Counter();
        new Counter();
        new Counter();
        Counter.displayCount();
    }
}
```





## OUTPUT:

<img width="557" height="252" alt="image" src="https://github.com/user-attachments/assets/e09ac8db-3c5e-4c3c-b1f2-b96450734be2" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
