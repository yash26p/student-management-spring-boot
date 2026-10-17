# Student Management Backend

A Spring Boot REST API for managing students with JWT-based authentication, MySQL database integration, Spring Data JPA, and CRUD operations.

## Features

- User Registration
- User Login
- JWT Token Generation
- JWT Authentication
- Add Student
- View All Students
- View Student by ID
- Update Student
- Delete Student
- MySQL Database Integration
- Spring Data JPA / Hibernate
- RESTful APIs
- Postman API Testing

## Technologies Used

- Java 25
- Spring Boot 4.1.1
- Spring Web
- Spring Security
- JWT
- Spring Data JPA
- Hibernate
- MySQL 8
- Maven
- Postman
- Git & GitHub

## Student Details

Each student contains:

- ID
- Name
- Email
- Branch
- Year

## API Endpoints

### Authentication

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login and generate JWT token |

### Student Management

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/students` | Add a new student |
| GET | `/api/students` | Get all students |
| GET | `/api/students/{id}` | Get student by ID |
| PUT | `/api/students/{id}` | Update student |
| DELETE | `/api/students/{id}` | Delete student |

## Authentication

The student APIs are protected using JWT authentication.

After successful login, the server generates a JWT token.

For protected APIs, use the token in the request header:

```text
Authorization: Bearer <JWT_TOKEN>
