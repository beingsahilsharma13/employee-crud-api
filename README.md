# 🚀 Employee CRUD REST API

A Spring Boot REST API for managing employees with full CRUD operations.

## Tech Stack
- Java 17
- Spring Boot 3.2
- Spring Data JPA
- H2 In-Memory Database
- Lombok
- Maven

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/employees | Create employee |
| GET | /api/employees | Get all employees |
| GET | /api/employees/{id} | Get employee by ID |
| GET | /api/employees/department/{dept} | Get by department |
| PUT | /api/employees/{id} | Update employee |
| DELETE | /api/employees/{id} | Delete employee |

## Sample Request Body

```json
{
  "firstName": "Sahil",
  "lastName": "Sharma",
  "email": "sahil@example.com",
  "department": "Engineering",
  "designation": "Backend Engineer",
  "salary": 80000
}
```

## Run Locally

```bash
mvn spring-boot:run
```

Visit H2 Console: http://localhost:8080/h2-console

## Built with ❤️ by Sahil Sharma
