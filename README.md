# Exp10-java
## Aim:
To code a program that produces output of power value for the corresponding base and exponnent.

## Algorithm:
### Step1:
Import the required packages.

### Step2:
Create a seperste methods for employee,manager and member.

### Step3:
Using extends method get the results.

### Step4:
And display it accordingly.
## Code:
```
import java.util.Scanner;
public class Main {
    public static void main(String[] args)
    {
        Scanner scan=new Scanner(System.in);
        Employee emp=new Employee();
        System.out.println("Enter employee details");
        emp.name= scan.next();
        emp.age= scan.nextInt();
        emp.phno= scan.nextLong();
        emp.address= scan.next();
        emp.specialisation= scan.next();
        emp.salary=scan.nextInt();

        Manager man=new Manager();
        System.out.println("Enter manager details");
        man.name= scan.next();
        man.age= scan.nextInt();
        man.phno= scan.nextLong();
        man.address= scan.next();
        man.department= scan.next();
        man.salary=scan.nextInt();

        System.out.println("The Employee Details are: \nName: "+emp.name+"\nAge: "+emp.age+"\nPhone number: "+emp.phno+"\nAddress:
        "+emp.address+"\nSpecialisation: "+emp.specialisation);
        emp.printSalary(emp.salary);
        System.out.println("The Manager Details are: \nName: "+man.name+"\nAge: "+man.age+"\nPhone number: "+man.phno+"\n
        Address: "+man.address+"\nDepartment:"+man.department);
        man.printSalary(man.salary);
    }
} 
```
```
public class Manager extends Member {
    String department;
}
```
```
public class Employee extends Member {
    String specialisation;
}
```
``` 
public class Member {
    String name;
    int age;
    long phno;
    String address;
    int salary;
    public void printSalary(int sal)
    {
        System.out.println("Salary: "+sal);
    }
}
```
## Output:
 ![image](https://github.com/Archana2003-Jkumar/Exp10-java/assets/93427594/e0373f92-7458-4a29-96a2-f09871dc08ad)

## Result:
Hence the program has been successfully executed.
