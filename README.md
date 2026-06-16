# student-management
# Student Management System

A Spring Boot-based Student Management System that provides REST APIs for managing student records. The application uses Spring Boot, Spring Data JPA, MySQL, and Maven to perform CRUD operations on student data.

## Features

* Add new students
* View all students
* View student details by ID
* Update student information
* Delete student records
* RESTful API architecture
* MySQL database integration
* Spring Data JPA persistence layer

## Tech Stack

* Java 17
* Spring Boot 3.2
* Spring Data JPA
* MySQL
* Maven
* Hibernate

## Project Structure

```
src
├── main
│   ├── java
│   │   └── com.example.studentmanagement
│   └── resources
│       └── application.properties
└── test
```

## Prerequisites

Before running the application, ensure you have:

* Java 17+
* Maven 3.9+
* MySQL Server

## Database Setup

Create a MySQL database:

```sql
CREATE DATABASE student_management;
```

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/student_management
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## Installation

Clone the repository:

```bash
git clone https://github.com/xionsammy/student-management.git
cd student-management
```

Build the project:

```bash
mvn clean install
```

Run the application:

```bash
mvn spring-boot:run
```

Or:

```bash
java -jar target/student-management-1.0.0.jar
```

## API Endpoints

| Method | Endpoint       | Description          |
| ------ | -------------- | -------------------- |
| GET    | /students      | Get all students     |
| GET    | /students/{id} | Get student by ID    |
| POST   | /students      | Create a new student |
| PUT    | /students/{id} | Update student       |
| DELETE | /students/{id} | Delete student       |

### Example Student JSON

```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "course": "Computer Science"
}
```

## Running Tests

```bash
mvn test
```

Skip tests:

```bash
mvn clean package -DskipTests
```

## Future Enhancements

* Student search and filtering
* Pagination and sorting
* Authentication and authorization
* Swagger/OpenAPI documentation
* Docker support
* Frontend integration

## License

This project is licensed under the MIT License.

## Author

Samuel Xavier

GitHub: https://github.com/xionsammy

```
```
