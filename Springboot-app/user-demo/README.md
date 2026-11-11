# User Demo (Spring Boot)

Requirements: Java 17+, Maven 3.6+

## Run
    mvn spring-boot:run

## APIs

### 1. Create user
    curl -X POST http://localhost:8080/api/users/register \
      -H "Content-Type: application/json" \
      -d '{"name":"Ali","email":"ali@example.com","password":"secret123"}'

### 2. Login
    curl -X POST http://localhost:8080/api/users/login \
      -H "Content-Type: application/json" \
      -d '{"email":"ali@example.com","password":"secret123"}'
