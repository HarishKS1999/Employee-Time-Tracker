# Employee-Time-Tracker

. Introduction
The Employee Time Tracker application aims to help employees log, manage, and track their daily tasks and working hours. The system provides role-based access control (RBAC) to differentiate between Associate and Admin users, offering a secure and efficient way to handle task management and reporting.

2. Features
Task Management: Add, edit, and delete tasks with details such as Employee Name, Role, Project, Date, Time Duration, Task Category, and Description.
RBAC: Differentiates actions available to Associates and Admins.
Reporting and Charts: Provides daily, weekly, and monthly summaries and visualizations of tasks and hours.
Validation: Ensures no duplicate task entries and task durations are capped at 8 hours.

3. Use Cases

Employee (Associate):
Add, edit, and delete tasks.

Admin:
Add, edit, and delete tasks for any employee.

4. System Architecture
Frontend: JSP, HTML, CSS, JavaScript
Backend: Java Servlet, JSP
Database: MySQL
Charting Library: Google Charts or Chart.js

5. Module Breakdown
Authentication Module: Handles user login and role-based access.
Task Management Module: Manages CRUD operations for tasks.
Reporting Module: Generates and displays charts and reports.
Validation Module: Ensures data integrity and business rules.

6. Bill of Materials (BOM)
Software:
Java Development Kit (JDK) 11+
Apache Tomcat 10.0.27
MySQL 8.0+
Eclipse IDE
Google Charts or Chart.js
Hardware:
Development Machine: Minimum 8GB RAM, 256GB SSD
Server: Minimum 16GB RAM, 1TB SSD (Production Environment)

7. Implementation Details
Modular Code Structure:
Each module (Authentication, Task Management, Reporting) will have its own package.
DAO (Data Access Object) pattern for database interactions.
MVC (Model-View-Controller) architecture for clean separation of concerns.

8. Security Considerations
Only authenticated users can access the application.
User roles determine permissible actions.
All user inputs will be validated and sanitized to prevent SQL injection and XSS attacks.

Project Title: Employee Time Tracker
Description
A web application that allows employees to track their tasks and working hours, providing role-based access control and various reporting features.

Features

Add, edit, and delete tasks.
Role-based access control for Associates and Admins.
Daily, weekly, and monthly task reports with visualizations.
Validation to prevent duplicate entries and excessive task durations.
Installation

Set up the database:
Import the provided SQL script to create the necessary tables.
Configure the application:
Update the database configuration in dbconfig.properties.
Deploy the application:
Deploy the WAR file to Apache Tomcat.
Usage

Run the application:
Access the application via http://localhost:8080/Time/LoginPage.jsp

Login:
Use the credentials provided in the users.sql script.

Contribution
Feel free to submit pull requests or open issues for suggestions and improvements.
