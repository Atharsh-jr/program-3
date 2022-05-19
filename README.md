# program-
Mr John is working as data entry operator in company XYZ. He wants to gather the information 
about the new employees joining the organization. Design a java application to read and display the 
information about n employees.
Program
import java.util.Scanner;
class Employee
{
 int id,age;
 String name; 
 long salary;
void getData()
{
 Scanner sc = new Scanner(System.in);
 System.out.println("Enter Employee Id : "); 
 id = sc.nextInt();
 System.out.println("Enter Employee Name : "); 
 name = sc.next();
 System.out.print("Enter Employee Age : "); 
 age = sc.nextInt();
 System.out.print("Enter Employee Salary : "); 
 salary = sc.nextLong();
}
void putData()
{
System.out.println(id + "\t\t" +name + "\t\t" +age + "\t\t"+salary);
}
}
public class EmployeeObj
{
public static void main(String args[])
{
 int n;
 Scanner s = new Scanner(System.in);
 System.out.println("Enter the number of employees");
 n=s.nextInt();
 Employee[] Emp = new Employee[n]
 int i;
for(i=0;i<n;i++)
 Emp[i] = new Employee(); // Allocating memory to each object
 for(i=0;i<n;i++)
 {
 System.out.println("Enter details of Employee " + (i+1));
 Emp[i].getData();
 }
 System.out.println("Details of Employees\n");
 for(i=0;i<n;i++) 
 Emp[i].putData();
}
}
Output
Enter the numb
