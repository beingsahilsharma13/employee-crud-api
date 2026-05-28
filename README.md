# 🧑‍💼 Employee CRUD REST API

A Spring Boot REST API for managing employees. Built with Java 17, Spring Boot 3.2, JPA, and H2 in-memory database.

## 🚀 Tech Stack
- Java 17
- Spring Boot 3.2
- Spring Data JPA
- H2 In-Memory Database
- Lombok
- Bean Validation

## 📦 Project Structure
```
src/main/java/com/sahil/employee/
├── EmployeeApplication.java       # Main class
├── controller/
│   └── EmployeeController.java    # REST endpoints
├── service/
│   └── EmployeeService.java       # Business logic
├── repository/
│   └── EmployeeRepository.java    # DB operations
├── model/
│   └── Employee.java              # Entity
└── exception/
    ├── EmployeeNotFoundException.java
    └── GlobalExceptionHandler.java
```

## 🔗 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/employees` | Create new employee |
| GET | `/api/employees` | Get all employees |
| GET | `/api/employees/{id}` | Get employee by ID |
| GET | `/api/employees/department/{dept}` | Get by department |
| PUT | `/api/employees/{id}` | Update employee |
| DELETE | `/api/employees/{id}` | Delete employee |

## ▶️ How to Run
```bash
./mvnw spring-boot:run
```

## 🧪 Sample Request
```json
POST /api/employees
{
  "firstName": "Sahil",
  "lastName": "Sharma",
  "email": "sahil@example.com",
  "department": "Engineering",
  "salary": 75000
}
```

## 🗄️ H2 Console
Visit: http://localhost:8080/h2-console  
JDBC URL: `jdbc:h2:mem:employeedb`
