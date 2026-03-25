# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Circle with a private instance variable radius. Provide public getter and setter methods to access and modify the radius variable. However, provide two methods called calculateArea() and calculatePerimeter() that return the calculated area and perimeter based on the current radius value. 


import java.util.Scanner;

class Circle {
   
    private double radius;

  
    public double getRadius() {
        return radius;
    }

   
    public void setRadius(double radius) {
        this.radius = radius;
    }

    
    public double calculateArea() {
        return Math.PI * radius * radius;
    }

   
    public double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

//continue your code here

## AIM:
To write a Java program that demonstrates the use of getters, setters, and methods in a class by creating a Circle class to calculate and display the radius, area, and perimeter of a circle based on user input.

## ALGORITHM :
1. Define a class Circle with a private variable radius.

2. Create a getter method getRadius() to return the value of radius.

3. Create a setter method setRadius(double radius) to assign a value to the radius variable.

4. Define a method calculateArea() that returns the area of the circle using the formula πr².

5. Define a method calculatePerimeter() that returns the perimeter of the circle using the formula 2πr.

6. In the main method, create a Scanner object to read the radius from the user.

7. Read the radius value and store it in a variable.

8. Create an object of the Circle class and set the radius using the setter method.

9. Display the radius, area, and perimeter using the getter and calculation methods.

10. End the program after printing the results.




## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Circle {
    private double radius;

    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }

    public double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double radiusInput = sc.nextDouble();

        Circle circle = new Circle();
        circle.setRadius(radiusInput);

        System.out.printf("Radius: %.2f\n", circle.getRadius());
        System.out.printf("Area: %.2f\n", circle.calculateArea());
        System.out.printf("Perimeter: %.2f\n", circle.calculatePerimeter());
    }
}
```





## OUTPUT:
<img width="553" height="353" alt="image" src="https://github.com/user-attachments/assets/ed3500b0-102c-4009-a4f5-ebcad9d29755" />




## RESULT:
The program has been executed successfully and the desired output has been obtained.
