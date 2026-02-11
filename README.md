# Student Management REST API

A **Spring Boot-based RESTful API** for managing student records with full CRUD operations.  
This project demonstrates a clean **layered architecture** using Spring Boot, Spring Data JPA, and MySQL.

---

## Features

- Create a new student
- Retrieve all students
- Retrieve student by ID
- Update student details
- Delete student
- Layered Architecture (Controller → Service → Repository → Database)
- MySQL integration using Spring Data JPA
- RESTful API design

---

## Project Architecture

```
Client (Browser / Postman)
        ↓
Controller Layer
        ↓
Service Layer
        ↓
Repository Layer
        ↓
MySQL Database
```

### Layers Explained

- **Controller** → Handles HTTP requests
- **Service** → Contains business logic
- **Repository** → Handles database operations
- **Entity** → Maps Java objects to database tables

---

## Tech Stack

- **Java 21**
- **Spring Boot 3**
- **Spring Data JPA**
- **MySQL**
- **Maven**
- **Git & GitHub**

---

## Project Structure

```
src
 └── main
      ├── java/com/akshaya/student_management
      │      ├── controller
      │      ├── service
      │      ├── repository
      │      └── entity
      └── resources
```

---

## Setup & Installation

### 1️.Clone the Repository

```bash
git clone https://github.com/akshayavardhini/student-management-springboot.git
cd student-management-springboot
```

### 2️.Configure Database

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/student_db
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### 3️.Run the Application

```bash
./mvnw spring-boot:run
```

Application runs on:

```
http://localhost:8080
```

---

## API Endpoints

### Create Student

```
POST /api/students
```

Body:
```json
{
  "name": "Lokesh",
  "email": "lokesh@gmail.com",
  "course": "Spring Boot"
}
```

---

### Get All Students

```
GET /api/students
```

---

### Get Student By ID

```
GET /api/students/{id}
```

---

### Update Student

```
PUT /api/students/{id}
```

---

### Delete Student

```
DELETE /api/students/{id}
```

---

## Learning Outcomes

Through this project, I learned:

- Building REST APIs using Spring Boot
- Implementing layered architecture
- Using Spring Data JPA for database interaction
- Connecting Java applications to MySQL
- Managing version control using Git & GitHub

---

## Future Improvements

- Exception Handling with proper HTTP status codes
- Validation using Hibernate Validator
- DTO implementation
- Pagination & Sorting
- Unit Testing
- Deployment to cloud platform

---

## Authors

**Akshaya Vardhini**  
Pre-Final Year M.Tech Integrated Software Engineering Student, VIT  
Machine Learning | Data Science | Web Development 

---

⭐ If you found this project useful, feel free to star the repository!
