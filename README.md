# SQL-Filtering-Data
CREATE DATABASE MySchool;

USE MySchool;

CREATE TABLE Students (
  StudentID INT PRIMARY KEY AUTO_INCREMENT,
  FirstName VARCHAR(255) NOT NULL,
  LastName VARCHAR(255) NOT NULL,
  Age INT NOT NULL,
  Grade CHAR(1) NOT NULL
);
INSERT INTO Students (FirstName, LastName, Age, Grade)
VALUES ('John', 'Doe', 22, 'B'),
       ('Jane', 'Smith', 28, 'A'),
       ('Alice', 'Johnson', 19, 'C'),
       ('Bob', 'Williams', 30, 'B'),
       ('Charlie', 'Brown', 21, 'A');
SELECT *
FROM Students
WHERE Age > 25;
SELECT DISTINCT Age
FROM Students;
