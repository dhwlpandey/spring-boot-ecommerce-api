# Spring Boot E-Commerce API

RESTful backend API for managing e-commerce products using Spring Boot, Hibernate, and PostgreSQL.

## Features

* CRUD operations for products
* Product image upload and retrieval
* Keyword-based product search
* PostgreSQL persistence with Spring Data JPA

## Tech Stack

* Java 21
* Spring Boot
* Spring Data JPA
* Hibernate
* PostgreSQL
* Maven
* Lombok

## Setup

### Clone Repository

```bash
git clone https://github.com/dhwlpandey/spring-boot-ecommerce-api.git
cd spring-boot-ecommerce-api
```

### Create Database

```sql
CREATE DATABASE ecommerce_db;
```

### Configure Environment Variables

```text
DB_URL=jdbc:postgresql://localhost:5432/ecommerce_db
DB_USERNAME=postgres
DB_PASSWORD=your_password
```

### Run Application

```bash
./mvnw spring-boot:run
```

API Base URL:

```text
http://localhost:8080/api
```

## Main Endpoints

| Method | Endpoint                               |
| ------ | -------------------------------------- |
| GET    | /api/products                          |
| GET    | /api/product/{id}                      |
| POST   | /api/product                           |
| PUT    | /api/product/{id}                      |
| DELETE | /api/product/{id}                      |
| GET    | /api/products/search?keyword={keyword} |

## Future Improvements

* Request validation
* Global exception handling
* JWT authentication
* Pagination and sorting
* Swagger/OpenAPI documentation

## Author

Dhawal Pandey
