# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Write a class Animal with a method speak() that prints "I am an animal". Create an object and call the method.

class prog {
    void speak() {
        // Code Here
    }

    public static void main(String[] args) {
        // Object creation and method call here
    }
}

For example:

Result
I am an animal


## AIM:
To write a Java program that demonstrates the concept of classes and methods by defining an Animal class with a speak() method and invoking it through an object.

## ALGORITHM :
1. Define a class named Animal that contains a method called speak().

2. Inside the speak() method, print a message stating "I am an animal".

3. Create another class named prog that contains the main method.

4. Inside the main method, create an object of the Animal class.

5. Call the speak() method using the created object.

6. Execute the program to display the output.




## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
class Animal {
    void speak() {
        System.out.println("I am an animal");
    }
}

class prog {
    public static void main(String[] args) {
        Animal a = new Animal();
        a.speak();
    }
}

```





## OUTPUT:
<img width="443" height="236" alt="image" src="https://github.com/user-attachments/assets/9c3a34f3-db6d-45bf-9263-b4fb4987c3a2" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.
