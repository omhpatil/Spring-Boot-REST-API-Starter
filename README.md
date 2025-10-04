# 🧩 Spring Boot REST API Starter Project

A **Spring Boot** RESTful API starter project built with **Spring Boot 3**, **Spring Data JPA**, **MySQL**, and **ModelMapper**.  
This template is designed to help you quickly build scalable backend APIs with clean architecture and DTO–Entity mapping.

---

## ✨ Features

* **CRUD Ready:** Easily add create, read, update, and delete operations.
* **DTO & Entity Mapping:** Uses **ModelMapper** to convert between entities and DTOs cleanly.
* **Validation:** Includes support for data validation using `@Valid` and `jakarta.validation` annotations.
* **Spring Data JPA:** Simplifies database operations.
* **Exception Handling:** Can be extended with `@ControllerAdvice` for global exception handling.
* **Lombok:** Reduces boilerplate code for getters, setters, and constructors.

---

## 🧰 Technologies Used

* **Java:** 21+
* **Spring Boot:** 3.5.6
* **Spring Data JPA**
* **ModelMapper**
* **MySQL**
* **Lombok**
* **Maven**

---

## 📘 API Endpoint Table

| **HTTP Method** | **Endpoint**         | **Description**             | **Request Body** | **Response (Status Code)** | **Example Response** |
|------------------|----------------------|-----------------------------|------------------|-----------------------------|----------------------|
| **POST** | `/api/users` | Create a new user | ✅ Required | **201 Created** | `{ "id": 1, "name": "Om Patil", "email": "om@example.com", "age": 22 }` |
| **GET** | `/api/users` | Get all users | ❌ Not required | **200 OK** | `[ { "id": 1, "name": "Om Patil", "email": "om@example.com", "age": 22 } ]` |
| **GET** | `/api/users/{id}` | Get user by ID | ❌ Not required | **200 OK** / **404 Not Found** | `{ "id": 1, "name": "Om Patil", "email": "om@example.com", "age": 22 }` |
| **PUT** | `/api/users/{id}` | Update existing user | ✅ Required | **200 OK** / **404 Not Found** | `{ "id": 1, "name": "Om P.", "email": "ompatil@example.com", "age": 23 }` |
| **DELETE** | `/api/users/{id}` | Delete user by ID | ❌ Not required | **200 OK** / **404 Not Found** | `{ "message": "User deleted successfully", "status": "SUCCESS" }` |
