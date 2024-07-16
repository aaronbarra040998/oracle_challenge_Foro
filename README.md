# CHALLENGE FORO HUB

Project Challenge from the Java and Spring Boot course by Alura/Oracle. It consists of a REST API that simulates a forum to solve doubts related to certain courses. The forum includes topics, topic responses, courses, and users.

## Description

Create a forum called ForoHub: develop a REST API using Spring to manage topics, responses, courses, and users. The API should allow:

- Create, read, update, and delete topics, responses, and users (CRUD).
- Implement a relational database for persistence.
- Authentication/authorization service to restrict access.

## Technologies Used

- Java JDK v17
- Maven v4
- Spring Boot v3.2.6
- Spring Data JPA
- Spring Security
- Spring Web
- SpringDoc-OpenAPI
- Auth0
- MySQL v8
- Flyway Migration
- Validation
- Lombok

## Project Features

1. User registration
2. User login
3. User listing, updating, and deletion
4. CRUD for topics
5. CRUD for responses
6. Authentication required for CRUD operations

## Code Comments

### REST Model Best Practices

- MVC Pattern: Data for Topics, Responses, Courses, and Users are in the Domain package. Controllers communicate with the REST Client.
- Use of Spring's ResponseEntity with DTOs.

### Validations

- Business validations: Avoid duplicate topics and enforce user registration restrictions.
- Integrity validations: Use ValidacionDeIntegridad for exceptions.

### Error Handling

- Configuration to avoid exposing sensitive stacktrace information.
- TratadorDeErrores class to capture exceptions and handle errors (400, 404, etc.).

### Database

- Use of MySQL as the database manager.

### Authentication/Authorization

- Authentication with email and password using Spring Security.
- Generation and verification of JWT with Auth0.
- Authorization with tokens in the header of each REST API request.

## Deployment

1. Clone the repository.
2. Import the project into a Java-supporting IDE.
3. Create the "foro-api" database in MySQL.
4. Configure environment variables in application.properties.
5. Run the project.
6. Create and test requests in Insomnia or Postman.
7. Test the project with SpringDoc using Swagger.
