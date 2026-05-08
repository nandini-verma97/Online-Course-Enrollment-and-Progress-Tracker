# Online-Course-Enrollment-and-Progress-Tracker
Project Overview
This project is a database management system designed for an online learning platform.
It manages course enrollments, tracks student progress, and generates performance reports using SQL and DBMS concepts.
The project focuses on:
Relational database design
SQL implementation
Stored procedures
Views and reporting
Data integrity using primary and foreign keys

Technologies Used
MySQL
SQL
DBMS Concepts

Features
Student course enrollment
Progress tracking for lessons
Performance report generation
Course-wise enrollment analytics
Stored procedures for automation
SQL views for reporting



Database Tables
Users
Stores student, instructor, and admin details.
Fields
id
name
email
role

Courses
Stores course information.
Fields
id
title
instructor_id

Lessons
Stores lessons for each course.
Fields
id
course_id
title

Enrollments
Stores student enrollments in courses.
Fields
id
user_id
course_id
date_of_enroll

Progress
Tracks lesson completion and scores.
Fields
id
enrollment_id
lesson_id
status
score



Stored Procedures
EnrollStudent
Enrolls a student into a course.
InsertUser
Adds a new user to the system.
UpdateProgress
Updates lesson progress and score.

Views
StudentPerformance
Displays average score of students.
CourseEnrollment
Displays total enrollments per course.

ER Diagram
The project contains the following entity relationships:
Users → Enrollments (1:N)
Courses → Enrollments (1:N)
Courses → Lessons (1:N)
Enrollments → Progress (1:N)
Lessons → Progress (1:N)

How to Run
Open MySQL.
Create a database.
Import the project.sql file.
Execute the SQL script.
Run queries and stored procedures.


Sample Stored Procedure Call
CALL EnrollStudent(1,2);

Author
Nandini Verma
