# Ex.No:3(b) POLYMORPHISM

## QUESTION:

Write a Java program to create a class Vehicle with a method called speedUp(). Create two subclasses Car and Bicycle. Override the speedUp() method in each subclass to increase the vehicle's speed differently.

For example:

Input	Result
car
10
Car speed increased to: 20 km/h

## AIM:
To write a Java program that demonstrates method overriding and runtime polymorphism by defining different types of vehicles (Car and Bicycle) that accelerate differently using overridden speedUp() methods.

## ALGORITHM :
1. Define a base class Vehicle with an integer variable speed and a method speedUp(int increment) that increases the speed.

2. Create a subclass Car that overrides the speedUp() method to increase speed at twice the given increment and prints the updated speed.

3. Create another subclass Bicycle that overrides the speedUp() method to increase speed normally and prints the updated speed.

4. In the main method, create a Scanner object to read the vehicle type and speed increment from the user.

5. Read the user input for vehicle type and the increment value.

6. Based on the type entered, create an object of Car or Bicycle.

7. If the input type is invalid, print an error message and terminate the program.

8. Call the speedUp() method on the selected vehicle object to apply acceleration.

9. Display the result using the overridden method.




## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class Vehicle {
    int speed;

    void speedUp(int increment) {
        speed += increment;
    }
}

class Car extends Vehicle {
    @Override
    void speedUp(int increment) {
        speed += increment * 2; // Car accelerates faster
        System.out.println("Car speed increased to: " + speed + " km/h");
    }
}

class Bicycle extends Vehicle {
    @Override
    void speedUp(int increment) {
        speed += increment; // Bicycle accelerates normally
        System.out.println("Bicycle speed increased to: " + speed + " km/h");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String type = sc.nextLine().trim();
        int increment = sc.nextInt();

        Vehicle vehicle;

        if (type.equalsIgnoreCase("car")) {
            vehicle = new Car();
        } else if (type.equalsIgnoreCase("bicycle")) {
            vehicle = new Bicycle();
        } else {
            System.out.println("Invalid vehicle type");
            return;
        }

        vehicle.speedUp(increment);
    }
}

```



## OUTPUT:

<img width="781" height="370" alt="image" src="https://github.com/user-attachments/assets/7b2b157d-9370-4564-85a7-4f5ec5ae2ce8" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
