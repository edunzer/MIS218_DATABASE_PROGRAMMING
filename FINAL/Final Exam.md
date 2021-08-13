## FINAL EXAM

Question 1
1 / 1 pts
Which of the following clauses would you use to identify the data source for a query?
  from 

 
UnansweredQuestion 2
0 / 1 pts
A query that isn’t executed when it’s defined uses ____________________ execution.
 
IncorrectQuestion 3
0 / 1 pts
Consider the following code example:
 
public class Department
{
    public int DepartmentID;
    public string DepartmentName;
    public string Chairman;
}
 
public class Student
{
    public int StudentID;
    public string LastName;
    public string FirstName;
    public int DepartmentID;
    public int UnitsCompleted;
}
 
What data will be returned when the following method-based query is executed?
 
List<Student> studentList = StudentDB.GetStudents();
var students = studentList
               .OrderByDescending(i => i.UnitsCompleted)
               .ThenBy(i => i.LastName)
               .ThenBy(i => i.FirstName)
               .Select(i => new { i.UnitsCompleted, i.LastName,
                   i.FirstName });
 
  
  The UnitsCompleted, LastName, and FirstName fields from all the Student objects sorted by the UnitsCompleted field in descending sequence within the LastName field within the FirstName field 
 
Question 4
1 / 1 pts
Consider the following code example:
 
public class Department
{
    public int DepartmentID;
    public string DepartmentName;
    public string Chairman;
}
 
public class Student
{
    public int StudentID;
    public string LastName;
    public string FirstName;
    public int DepartmentID;
    public int UnitsCompleted;
}
 
What data will be returned when the following query expression is executed?
 
List<Student> studentList = StudentDB.GetStudents();
var students = from student in studentList
               where student.UnitsCompleted > 50
               orderby student.DepartmentID,
                       student.UnitsCompleted descending
               select student;
 
  All Student objects with units completed greater than 50 

 
IncorrectQuestion 5
0 / 1 pts
An anonymous type is created for the results of a query when

  a query returns selected elements from the data source 

 
Question 6
1 / 1 pts
Consider the following code example:
 
public class Department
{
    public int DepartmentID;
    public string DepartmentName;
    public string Chairman;
}
 
public class Student
{
    public int StudentID;
    public string LastName;
    public string FirstName;
    public int DepartmentID;
    public int UnitsCompleted;
}
 
What data will be returned when the following query expression is executed?
 
List<Student> studentList = StudentDB.GetStudents();
List<Department> departmentList = DepartmentDB.GetDepartments();
var students = from student in studentList
               join department in departmentList
               on student.DepartmentID equals department.DepartmentID
               orderby department.DepartmentName, student.LastName,
                       student.FirstName
               select new { department.DepartmentName,
                            student.LastName, student.FirstName };
 
  The DepartmentName field from all the Department objects with matching DepartmentID fields in one or more Student objects, and the LastName and FirstName fields from all the  matching Student objects 
 
Question 7
1 / 1 pts
To execute a query, you typically code a
  foreach statement 

 
Question 8
1 / 1 pts
The query operators provided by LINQ are implemented as ____________________ methods.
extension 
 
IncorrectQuestion 9
0 / 1 pts
To identify the data you want to retrieve from a data source, you can define a method-based query or a query ____________________.
dataset
 
IncorrectQuestion 10
0 / 1 pts
In an SDI application, each form runs in its own ___________.
instance
 
Question 11
1 / 1 pts
To add menus to a form, you need to add a _______________ control to the form.
menustrip
 
Question 12
1 / 1 pts
On a Tab control, what event occurs when the user selects another tab?

  SelectedIndexChanged
 
Question 13
1 / 1 pts
To add a toolbar to a form, you need to add a ______________ control to the form.
toolstrip
 
Question 14
1 / 1 pts
What menu item property determines if the menu item is grayed out?

  Enabled 

 
Question 15
1 / 1 pts
What control must you add to a form if you want to display a brief description of a control on the form when you place the mouse pointer over it?

  ToolTip 
 
Question 16
1 / 1 pts
When you use a multiple-document interface, what type of form contains the other forms?
  a parent form 

 
IncorrectQuestion 17
0 / 1 pts
To add context-sensitive help to a form, you need to add a ______________ control to the form.
tooltip
 
IncorrectQuestion 18
0 / 1 pts
To install a commercial application that’s delivered on a CD or DVD, you would probably use _____________________ deployment.
InstallAware
 
Question 19
1 / 1 pts
When you use a Setup program for deployment, the user starts the installation by double-clicking on the _________________ file.
setup.exe
 
Question 20
1 / 1 pts
By default, ClickOnce deployment provides for automatic updates, and the users are alerted
  when they start the application and an update is available 

 
Question 21
1 / 1 pts
Which of the following is not a feature of Setup program deployment?
  It provides for automatic updating of the application. 

 
Question 22
1 / 1 pts
An easy way to configure a Setup program is to

  use the InstallShield Project Assistant 
 
Question 23
1 / 1 pts
When you’re deploying an application that uses a SQL Server database on a network server, you need to

  make sure the connection string is set correctly 
 
Question 24
1 / 1 pts
To distribute a Setup program to the users, you can

  both a and b 
 
IncorrectQuestion 25
0 / 1 pts
For all but the simplest of installations, you probably wouldn’t use _____________________ deployment.
Windows Installer XML
