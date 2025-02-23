# Overview
A RESTful API service built using Spring Boot provides endpoints for Registration and Login and other functionalities, using MySQL to persist the data.

# Features
* Authentication and Authorization : Implemented using Bearer token.
* User management:
  + User registration with email, password (encrypted using BCrypt), first name, last name
  + User login using email and password and a bearer token will get generated.
* User Task management:
  + Create, update and delete users.

# Getting Started:
## Prerequisites:
* Java 17 or higher
* MySql
* Postman for API Testing

## Configuration:
1. Open the application.properties file located in src/main/resources directory.
2. Configure the MySQL database connection settings:
   
   spring.datasource.url = jdbc:mysql://localhost:3306/yourdbname
   
   spring.datasource.username = root
   
   spring.datasource.password = password

   Replace localhost, 3306, root and password with your MySQL host, port, username and password respectively.

   Save the changes to the application.properties file.

## Running the application:
Run the application using Gradle:
./gradlew bootrun
