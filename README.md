# Authentication & Authorization API with Spring Boot

## Objective

Develop an **Authentication / Authorization (Login API)** using **Java** and the **Spring Boot** framework.

## Requirements

The application should support user login using **username** and **password**. Upon successful login, the system must authenticate the user and authorize access to specific API endpoints based on their assigned role.

### API Endpoints

| Endpoint | Description |
|----------|-------------|
| `POST /login` | Handle user authentication. |
| `GET /user`  | Accessible based on user role. You can design the response as needed. |
| `GET /admin` | Accessible only to users with an `ADMIN` role. Response can be designed freely. |

### Authorization Rules

- If the authenticated user has the role **ADMIN**:
  - Access is granted to all three endpoints: `/login`, `/user`, and `/admin`.

- If the authenticated user has the role **USER**:
  - Access is restricted to only `/login` and `/user`.

## Development Guidelines

- You may choose any development approach, architecture, and libraries as you see fit.
- Suggested tools/libraries (optional):
  - Spring Security
  - JWT (JSON Web Tokens)
  - OAuth2
  - Lombok
  - Spring Data JPA / Hibernate

## Bonus Points

Additional features or enhancements that demonstrate:
- **Security best practices**
- **Performance optimization**
- **Clean architecture and code quality**
- **Instructions to run and test the application (e.g., via Postman or Swagger)**

...will be considered for special recognition.

## Deliverables
- Source code (Using your GitHub repository)

