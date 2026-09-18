# Library Management REST API

A beginner-friendly backend project built with **Java, Spring Boot, Spring Data JPA, REST APIs, and MySQL**.

## Features
- Add a book
- Get all books
- Get a book by ID
- Update a book
- Delete a book
- Search books by title or author
- MySQL database persistence
- Validation and global exception handling

## Tech Stack
- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA / Hibernate
- MySQL
- Maven
- REST API
- Postman

## Project Structure
```
src/main/java/com/harshith/library
├── LibraryManagementApplication.java
├── controller/BookController.java
├── entity/Book.java
├── exception/BookNotFoundException.java
├── exception/GlobalExceptionHandler.java
├── repository/BookRepository.java
└── service/BookService.java
```

## Database Setup
Create a MySQL database:
```sql
CREATE DATABASE library_db;
```

Update `src/main/resources/application.properties` with your local MySQL username and password.

## API Endpoints
| Method | Endpoint | Purpose |
|---|---|---|
| POST | /api/books | Add a book |
| GET | /api/books | Get all books |
| GET | /api/books/{id} | Get book by ID |
| PUT | /api/books/{id} | Update a book |
| DELETE | /api/books/{id} | Delete a book |
| GET | /api/books/search?keyword=java | Search books |

## Example JSON
```json
{
  "title": "Effective Java",
  "author": "Joshua Bloch",
  "isbn": "9780134685991",
  "available": true
}
```

## Run
```bash
mvn spring-boot:run
```

The application runs on port 8080.
