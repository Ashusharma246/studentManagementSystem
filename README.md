Student Management System
Welcome to the Student Management System! This project is designed to help you manage student records easily and efficiently. Built with Spring Boot and MySQL, it provides a simple interface to add, update, delete, and view student information.

What Can You Do?
Add Students: Quickly add new students with details like name, email, course, and status.
Update Info: Need to change a student’s details? No problem—just edit their record.
Delete Students: Easily remove students from the system.
View All Students: See a list of all students in the system.
Search: Look up specific students with the search feature.
Technology Behind the Scenes
Backend: Spring Boot and Spring Data JPA handle the heavy lifting.
Frontend: We’ve kept it simple with Thymeleaf, HTML, and CSS for a clean, easy-to-use interface.
Database: MySQL stores all the student data.
Build Tool: Maven for managing dependencies and building the project.
How to Get Started
What You Need
Java 11 or higher
MySQL Server installed
Maven for building the project
Your favorite IDE (like IntelliJ or Eclipse)
Step-by-Step Guide
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/Ashusharma246/studentManagementSystem.git
cd student-management-system/student-management-system
Set up the MySQL database:

Open MySQL Workbench (or use the MySQL command line).

Create a new database called student_management_system:

sql
Copy code
CREATE DATABASE student_management_system;
Configure the database connection in application.properties (you’ll find this in the src/main/resources/ folder):

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/student_management_system
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Build the project using Maven:

bash
Copy code
mvn clean install
Run the application:

bash
Copy code
mvn spring-boot:run
Open your browser and go to http://localhost:8080 to access the app.

Endpoints to Explore
/students: View the full list of students.
/students/add: Add a new student to the system.
/students/edit/{id}: Edit details of a specific student.
/students/delete/{id}: Delete a student from the database.
