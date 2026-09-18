Student Marks & Grade Management System 
A console-based Java application developed as a Programming in Java project. The 
system manages student information and academic marks and automatically generates 
total marks, percentage, and grade. 
Project Overview 
The Student Marks & Grade Management System is designed to simplify the 
management of student academic records. 
The application allows users to: 
• Add student details 
• Store marks for multiple subjects 
• Display all student records 
• Search students using roll number 
• Generate student results 
• Calculate total marks 
• Calculate percentage 
• Calculate grade 
• Delete student records 
• Validate user input 
• Handle invalid input using exception handling 
• Generate reports using multithreading 
The project demonstrates important concepts from the Programming in Java course, 
including Java fundamentals, Object-Oriented Programming, Collections, Exception 
Handling, and Multithreading. 
Objectives 
The main objectives of this project are: 
1. To develop a practical Java application using object-oriented programming. 
2. To manage multiple student records efficiently. 
3. To calculate student results automatically. 
4. To reduce manual calculation errors. 
5. To demonstrate exception handling and input validation. 
6. To demonstrate Java multithreading. 
7. To apply concepts from three major modules of Programming in Java. 
Features 
1. Add Student 
The user can add: 
• Roll Number 
• Student Name 
• Course 
• Java Marks 
• DBMS Marks 
• Operating System Marks 
• Computer Networks Marks 
• Mathematics Marks 
2. Display Students 
Displays all students currently stored in the system along with their percentage. 
3. Search Student 
Students can be searched using their roll number. 
4. Generate Result 
The system calculates: 
Total Marks 
Percentage 
Grade 
5. Delete Student 
A student can be deleted using their roll number. 
6. Input Validation 
The system validates: 
• Roll number 
• Student name 
• Marks 
Marks must be between: 
0 - 100 
7. Exception Handling 
The project handles invalid input using Java exception handling mechanisms such as: 
try 
catch 
throw 
IllegalArgumentException 
InputMismatchException 
8. Multithreading 
A separate ReportThread is used to generate the student's result report. 
Technologies Used 
Technology 
Java 
ArrayList 
OOP 
Usage 
Main programming language 
Store student objects 
Application structure 
Exception Handling Input validation and error handling 
Multithreading 
Scanner 
GitHub 
Report generation 
User input 
Source code management 
Java Concepts Covered 
Module 1 – Java Fundamentals 
• Variables 
• Data types 
• Operators 
• Input and Output 
• Scanner 
• Conditional statements 
• if-else 
• switch 
• Loops 
Module 2 – Object-Oriented Programming 
• Classes 
• Objects 
• Constructors 
• Encapsulation 
• Inheritance 
• super 
• Method overriding 
• Polymorphism 
• ArrayList 
Module 3 – Exception Handling and Multithreading 
• Exception handling 
• try-catch 
• throw 
• IllegalArgumentException 
• InputMismatchException 
• Thread creation 
• Thread 
• run() 
• start() 
• sleep() 
• InterruptedException 
Project Structure 
Student-Marks-Grade-Management-System/ 
│ 
├── Main.java 
├── Person.java 
├── Student.java 
├── Marks.java 
├── Result.java 
├── StudentManager.java 
├── InputValidator.java 
├── ReportThread.java 
│ 
├── README.md 
└── statement.md 
Class Responsibilities 
Main.java 
Controls the main menu and handles user interaction. 
Person.java 
Base class containing common person information. 
Student.java 
Represents a student and stores: 
• Roll number 
• Name 
• Course 
• Marks 
Marks.java 
Stores subject marks and performs mark-related calculations. 
Result.java 
Calculates and displays: 
• Total 
• Percentage 
• Grade 
StudentManager.java 
Manages the student collection using ArrayList. 
Provides operations such as: 
Add 
Search 
Display 
Delete 
InputValidator.java 
Validates user input and throws exceptions when invalid data is entered. 
ReportThread.java 
Extends the Java Thread class and generates the student report in a separate thread. 
 
    Application Workflow 
              START 
                | 
                ↓ 
          Display Main Menu 
                | 
                ↓ 
       Select an Operation 
                | 
       ┌────────┼─────────┐ 
       ↓        ↓         ↓ 
     Add      Search    Generate 
   Student    Student    Result 
       |        |         | 
       ↓        ↓         ↓ 
    Validate  Find      Calculate 
     Input    Student    Result 
       |                  | 
       └────────┬─────────┘ 
                ↓ 
          Display Output 
                | 
                ↓ 
          Return to Menu 
                | 
                ↓ 
               EXIT 
 
       Grade Calculation 
The system calculates the percentage using: 
Percentage = (Total Marks / 500) × 100 
The grade system used in the project is: 
Percentage Grade 
90 and above A+ 
80–89.99 
70–79.99 
60–69.99 
50–59.99 
40–49.99 
Below 40 
A 
B 
C 
D 
E 
F 
How to Run 
Prerequisites 
Install: 
• Java JDK 
• Any Java IDE such as IntelliJ IDEA, Eclipse, NetBeans, or VS Code 
Check Java installation: 
java -version 
Method 1 — Using an IDE 
1. Clone or download this repository. 
2. Open the project in your Java IDE. 
3. Make sure all .java files are in the same project/package. 
4. Open Main.java. 
5. Run Main.java. 
Method 2 — Using Command Prompt 
Open the project directory: 
cd Student-Marks-Grade-Management-System 
Compile: 
javac *.java 
Run: 
java Main 
Main Menu 
Example: 
======================================== 
STUDENT MARKS MANAGEMENT SYSTEM 
======================================== 
1. Add Student 
2. Display All Students 
3. Search Student 
4. Generate Result 
5. Delete Student 
6. Exit 
Enter your choice: 
Example Result 
========== STUDENT RESULT ========== ----- Student Details ----- 
Roll Number : 101 
Name       
Course     
 : Rahul 
 : B.Tech CSE 
------------- MARKS ------------- 
Java              
DBMS              
: 85.0 
: 78.0 
Operating System  : 90.0 
Computer Networks : 82.0 
Mathematics       : 88.0 ------------- RESULT ------------- 
Total      
: 423.0 / 500 
Percentage : 84.6% 
Grade      
: A 
Input Validation Example 
If the user enters: 
Java: 150 
The system displays: 
Error: Marks must be between 0 and 100. 
For an invalid roll number: 
Enter Roll Number: -5 
The system displays: 
Error: Roll number must be greater than 0. 
Multithreading 
The project demonstrates multithreading through: 
public class ReportThread extends Thread 
The report generation task is implemented inside: 
@Override 
public void run() 
The thread is started using: 
reportThread.start(); 
A short delay is simulated using: 
Thread.sleep(2000); 
Testing 
The following operations are tested: 
Test Case Description 
TC01 
TC02 
TC03 
TC04 
Add valid student 
Display students 
Search existing student 
Expected Result 
Student added 
Student details displayed 
Correct student displayed 
Search unavailable student Student not found 
TC05 
TC06 
TC07 
TC08 
TC09 
TC10 
TC11 
Enter marks > 100 
Enter negative marks 
Invalid numeric input 
Duplicate roll number 
Generate result 
Delete student 
Error displayed 
Error displayed 
Exception handled 
Duplicate rejected 
Total, percentage and grade displayed 
Student removed 
Generate threaded report Report generated using thread 
Limitations 
The current version has some limitations: 
• Data is stored only during program execution. 
• There is no database. 
• There is no graphical user interface. 
• There is no login/authentication system. 
• Student information is not permanently stored. 
Future Enhancements 
The project can be extended by adding: 
1. File Handling for permanent data storage. 
2. MySQL/JDBC for database connectivity. 
3. GUI using JavaFX or Swing. 
4. Student login and administrator login. 
5. Update/edit student records. 
6. Subject-wise performance reports. 
7. Class statistics. 
8. PDF report generation. 
9. Automated unit testing. 
Project Information 
Project: Student Marks & Grade Management System 
Course: Programming in Java 
Course Code: CSE2006 
Language: Java 
Project Type: Console-based Application 
Academic Year: 2026–27 
Project Documentation 
The complete project report contains: 
• Introduction 
• Problem Statement 
• Objectives 
• Functional Requirements 
• Non-functional Requirements 
• System Architecture 
• UML Diagrams 
• Workflow 
• Implementation Details 
• Testing 
• Challenges 
• Learnings 
• Future Enhancements 
• References 
License 
This project is developed for academic and educational purposes. 
