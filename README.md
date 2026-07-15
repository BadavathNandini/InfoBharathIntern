#Jewelry Backend Application

A secure RESTful backend application for managing a jewelry store, built using **Java**, **Spring Boot**, **Spring Security**, **JWT Authentication**, and **MySQL**.

##Project Overview

The Jewelry Backend Application provides secure user authentication and product management functionalities. It allows users to register, log in securely using JWT tokens, and perform CRUD operations on jewelry products through REST APIs.

This project was developed to strengthen backend development skills using the Spring Boot ecosystem.

---

##Features

###User Module
- User Registration
- User Login
- Password Encryption using BCrypt
- JWT Token Generation
- JWT Authentication
- User Profile API

###Product Module
- Add Product
- Get All Products
- Get Product by ID
- Update Product
- Delete Product
- Search Products by Name
- Filter Products by Category

---

## Tech Stack

- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- JWT (JSON Web Token)
- MySQL
- Maven
- Postman
- Swagger/OpenAPI

---

## Project Structure

src
├── controller
├── entity
├── repository
├── jwt
├── config
├── resources
└── JewelryBackendApplication.java

---

## Authentication

This project uses **JWT (JSON Web Token)** for authentication.

### Public APIs

```
POST /api/users/register
POST /api/users/login
```

### Protected APIs
GET    /api/users/profile

POST   /api/products
GET    /api/products
GET    /api/products/{id}
PUT    /api/products/{id}
DELETE /api/products/{id}
GET    /api/products/category/{category}
GET    /api/products/search/{name}

Protected APIs require a JWT token.

Example Authorization Header:
Authorization: Bearer <your_jwt_token>

---

##Database

Database Used:

- MySQL

Example database name:
jewelrydb
----

##How to Run

### Clone the Repository
git clone https://github.com/your-username/jewelry-backend.git


### Navigate to Project

cd jewelry-backend


### Configure Database

Update the `application.properties` file with your MySQL credentials.

Example:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/jewelrydb
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
----


### Run the Application

bash
mvn spring-boot:run


The application will start at:
http://localhost:8080
---




##API Testing

The APIs were tested using **Postman**.

### Workflow

1. Register User
2. Login User
3. Copy JWT Token
4. Add "Bearer Token" in Authorization
5. Access Protected APIs
----


##Sample APIs

### Register
POST /api/users/register

### Login
POST /api/users/login

### Get User Profile
GET /api/users/profile

### Get All Products
GET /api/products
----



##Learning Outcomes

- Spring Boot REST API Development
- Spring Security
- JWT Authentication
- Password Encryption using BCrypt
- MySQL Database Integration
- Hibernate & JPA
- RESTful API Design
- API Testing with Postman
- ---

##Future Enhancements

- Role-Based Authentication (Admin/User)
- Image Upload for Products
- Order Management
- Shopping Cart
- Payment Gateway Integration
- Docker Deployment
- Unit Testing
- CI/CD Pipeline
- ----

