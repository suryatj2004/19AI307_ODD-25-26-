# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:
Create a Student class and a StudentDAO interface with methods to add and retrieve students. Implement it with in-memory storage (ArrayList).

For example:

Input	Result
Muthu
21
CSE001
Muthu
21
CSE001

## AIM:
To write a Java program that demonstrates the DAO (Data Access Object) pattern by storing and retrieving Student objects using an interface and its implementation.

## ALGORITHM :
1. Create a Student class with private fields for name, age, and roll number, and provide getter methods.

2. Define a StudentDAO interface with methods addStudent() and getAllStudents().

3. Implement StudentDAO in a class StudentDAOImpl using an ArrayList to store Student objects.

4. In main(), create a Scanner to read input and a DAO object.

5. Read student details from the user and create a Student object.

6. Add the Student object to the DAO.

7. Retrieve all students from the DAO and display their details.

8. Close the Scanner.




## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.*;

class Student {
    private String name;
    private int age;
    private String rollNo;

    public Student(String name, int age, String rollNo) {
        this.name = name;
        this.age = age;
        this.rollNo = rollNo;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public String getRollNo() {
        return rollNo;
    }
}

interface StudentDAO {
    void addStudent(Student student);
    List<Student> getAllStudents();
}

class StudentDAOImpl implements StudentDAO {
    private List<Student> students = new ArrayList<>();

    public void addStudent(Student student) {
        students.add(student);
    }

    public List<Student> getAllStudents() {
        return students;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        StudentDAO dao = new StudentDAOImpl();

        String name = sc.nextLine();
        int age = Integer.parseInt(sc.nextLine());
        String rollNo = sc.nextLine();

        Student s = new Student(name, age, rollNo);
        dao.addStudent(s);

        for (Student student : dao.getAllStudents()) {
            System.out.println(student.getName());
            System.out.println(student.getAge());
            System.out.println(student.getRollNo());
        }

        sc.close();
    }
}

```





## OUTPUT:

<img width="487" height="431" alt="image" src="https://github.com/user-attachments/assets/d77f7f8c-10ea-4d85-a536-16c9d3b2cfa4" />


## RESULT:
The program has been executed successfully and the desired output has been obtained.
