# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create an abstract class TaxPayer with method calculateTax(). Create subclasses SalariedPerson and BusinessPerson.

For example:

Input	Result
1
50000
5000.00
1
72500
7250.00


## AIM:

To write a Java program that demonstrates abstraction and runtime polymorphism using an abstract class TaxPayer and its subclasses SalariedPerson and BusinessPerson, each calculating tax differently based on income.
## ALGORITHM :
1. Create an abstract class TaxPayer that declares an abstract method calculateTax().

2. Define a subclass SalariedPerson that extends TaxPayer, stores income, and implements calculateTax() by returning 10% of income.

3. Define another subclass BusinessPerson that extends TaxPayer, stores income, and implements calculateTax() by returning 15% of income.

4. In the main method, create a Scanner object to read user input.

5. Read the taxpayer type (1 for salaried, any other value for business) and the income amount.

6. Based on the type, create the appropriate subclass object and store it in a reference of type TaxPayer.

7. Use DecimalFormat to format the tax output to two decimal places.

8. Call the calculateTax() method using the object reference and print the formatted tax amount.

9. End the program.


## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:


```
import java.util.Scanner;
import java.text.DecimalFormat;

abstract class TaxPayer {
    abstract double calculateTax();
}

class SalariedPerson extends TaxPayer {
    double income;
    SalariedPerson(double income) { this.income = income; }
    double calculateTax() { return income * 0.10; }
}

class BusinessPerson extends TaxPayer {
    double income;
    BusinessPerson(double income) { this.income = income; }
    double calculateTax() { return income * 0.15; }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int type = sc.nextInt();
        double income = sc.nextDouble();
        TaxPayer person = (type == 1) ? new SalariedPerson(income) : new BusinessPerson(income);
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println(df.format(person.calculateTax()));
    }
}

```




## OUTPUT:
<img width="482" height="432" alt="image" src="https://github.com/user-attachments/assets/eff6bf74-8965-46f4-a94b-c5dbb4b2b8fe" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.
