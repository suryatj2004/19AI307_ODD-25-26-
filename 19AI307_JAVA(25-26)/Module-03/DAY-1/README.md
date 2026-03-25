# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:

A library wants to maintain records of its members. All members share some common information: a unique member ID, the member’s name, and the date when they joined the library (membershipDate).

There are two types of members:

StudentMember: In addition to the base information, they have the course they are enrolled in (courseEnrolled).

FacultyMember: In addition to the base information, they have the department they belong to (department).

Your task is to write a program that:

Reads exactly 4 member records.

Each record starts with the type of member: "Student" or "Faculty".

Then reads the required details according to the type.

Displays the details of all four membersInput Format:

Student
M101
Alice
2023-01-15
ComputerScience
import java.util.Scanner;

class Member {
    String memberId;
    String name;
    String membershipDate;

    Member(String memberId, String name, String membershipDate) {
        this.memberId = memberId;
        this.name = name;
        this.membershipDate = membershipDate;
    }

    void display() {
        System.out.println("Member ID: " + memberId);
        System.out.println("Name: " + name);
        System.out.println("Membership Date: " + membershipDate);
    }
}

//Continue your Code here
## AIM:
To write a Java program that demonstrates inheritance and polymorphism by creating a base class Member and two derived classes StudentMember and FacultyMember, storing multiple member objects in a list, and displaying their details dynamically based on their type.

## ALGORITHM :
1. Define a base class Member with attributes memberId, name, and membershipDate, along with a constructor and a display() method to print member details.

2. Create a subclass StudentMember that extends Member, adds the attribute courseEnrolled, and overrides the display() method to print additional details.

3. Create another subclass FacultyMember that extends Member, adds the attribute department, and overrides the display() method to print extra information.

4. In the main method, create a Scanner object to read input from the user.

5. Create an ArrayList to store objects of type Member.

6. Use a loop to continuously read input until an empty line is encountered.

7. For each entry, read the type (Student/Faculty), member ID, name, membership date, and additional field.

8. Based on the type, create either a StudentMember or FacultyMember object and add it to the list.

9. After collecting all inputs, iterate through the list of members.

10. Call the display() method on each object to print its details, demonstrating polymorphism.

11. End the program.





## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: SURYA T
RegisterNumber: 212222040168
*/
```

## SOURCE CODE:

```
import java.util.*;
class Member {
    String memberId;
    String name;
    String membershipDate;
    Member(String memberId, String name, String membershipDate) {
        this.memberId = memberId;
        this.name = name;
        this.membershipDate = membershipDate;
    }
    void display() {
        System.out.println("Member ID: " + memberId);
        System.out.println("Name: " + name);
        System.out.println("Membership Date: " + membershipDate);
    }
}
class StudentMember extends Member {
    String courseEnrolled;
    StudentMember(String memberId, String name, String membershipDate, String courseEnrolled) {
        super(memberId, name, membershipDate);
        this.courseEnrolled = courseEnrolled;
    }
    void display() {
        super.display();
        System.out.println("Student Member - Course Enrolled: " + courseEnrolled);
    }
}
class FacultyMember extends Member {
    String department;

    FacultyMember(String memberId, String name, String membershipDate, String department) {
        super(memberId, name, membershipDate);
        this.department = department;
    }
    void display() {
        super.display();
        System.out.println("Faculty Member - Department: " + department);
    }
}
public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        ArrayList<Member> members = new ArrayList<>();
        while (sc.hasNextLine()) {
            String type = sc.nextLine().trim();
            if (type.isEmpty()) break;
            String memberId = sc.nextLine().trim();
            String name = sc.nextLine().trim();
            String membershipDate = sc.nextLine().trim();
            String extra = sc.nextLine().trim();
            if (type.equalsIgnoreCase("Student")) {
                members.add(new StudentMember(memberId, name, membershipDate, extra));
            } else if (type.equalsIgnoreCase("Faculty")) {
                members.add(new FacultyMember(memberId, name, membershipDate, extra));
            }
        }
        
        for (Member m : members) {
            m.display();
            System.out.println();
        }
    }
}
```





## OUTPUT:
<img width="1308" height="550" alt="image" src="https://github.com/user-attachments/assets/4fc35b2b-6128-43c3-960e-73ea2652cf34" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.
