# Exercise 10

## AIM:
To write a java program that takes details from the parent class and executes the specified output.

## PROCEDURE:
1. Create a class called Member with instance variables for name, age, phone_number, address, and salary.
2. Inside the Member class, define a method named printSalary() that prints the value of salary.
3. Create a class called Employee that extends the Member class.
4. Inside the Employee class, define a method named emp() that prints the department of the employee.
5. Create a class called Manager that extends the Member class.
6. Inside the Manager class, define a method named emp1() that prints the specialization of the manager.
7. Create a class called Main.
8. Inside the Main class, define the main() method.
9. Inside the main() method, create an instance of the Employee class called e. Set the values for the member variables and call the emp() and printSalary() methods.
10. Similarly, create an instance of the Manager class called m. Set the values for the member variables and call the emp1() and printSalary() methods.

## PROGRAM:
```
public class Member {
    String name;

    int age;


    String phone_number;

    String address;

    int salary;
    public void printSalary()
    {

        System.out.println("Salary is:"+salary);

    }
}
public class Employee extends Member {


    public void emp() {

      String department="IT";
        System.out.print("Department of the emoployee: "+department+"\n");


    }
}
public class Manager extends Member {
    public void emp1() {

       String specialization="Front end developer.";
        System.out.println("specialization:"+specialization);

    }
}

Main Function:

public class Main {
    public static void main(String[] args)
    {
        Employee e=new Employee();
        System.out.println("Details of the employee:");
        e.name="Ashmi";
        e.age=23;
        e.phone_number="9567761840";
        e.address="T Nagar, Chennai.";
        e.salary=40000;
        System.out.println("Name: "+e.name);
        System.out.println("Age: "+e.age);
        System.out.println("Phone number: "+e.phone_number);
        System.out.println("Address: "+e.address);
        e.emp();
        e.printSalary();
        Manager m=new Manager();
        System.out.println("\nDeatils of the manager:");
        m.name="Rahul";
        m.age=34;
        m.phone_number="9897667839";
        m.address="Anna nagar,Chennai";
        m.salary=60000;
        System.out.println("Name: "+m.name);
        System.out.println("Age: "+m.age);
        System.out.println("Phone number: "+m.phone_number);
        System.out.println("Address: "+m.address);
        m.emp1();
        m.printSalary();

    }
}
```

## OUTPUT:

```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=4235:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\java java\out\production\java java" Emp
Details of the employee:
Name: Ashmi
Age: 23
Phone number: 9567761840
Address: T Nagar, Chennai.
Department of the emoployee: IT
Salary is:40000

Deatils of the manager:
Name: Rahul
Age: 34
Phone number: 9897667839
Address: Anna nagar,Chennai
specialization:Front end developer.
Salary is:60000

Process finished with exit code 0
```
