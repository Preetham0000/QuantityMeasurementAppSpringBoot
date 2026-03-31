# Quantity Measurement App - Spring Boot

A Spring Boot-based REST service for performing quantity measurements with support for comparison, conversion, and arithmetic operations with multiple measurement types (Length, Weight, Volume, Temperature).

#### Endpoint	Method	Description: 
- /compare	POST	Compare two quantities
- /convert	POST	Convert quantity to different unit
- /add	POST	Add two quantities
- /subtract	POST	Subtract quantities
- /multiply	POST	Multiply quantities
- /divide	POST	Divide quantities
- /history/operation/{type}	GET	Get measurements by operation type
- /history/type/{type}	GET	Get measurements by measurement type
- /history/errored	GET	Get failed operations
- /count/{operation}	GET	Count operations by type


#### Project Structure

| Directory | Purpose |
|-----------|---------|
| **controller/** | REST API endpoints and request/response handling |
| **service/** | Business logic and data processing layer |
| **repository/** | Spring Data JPA data access layer |
| **model/** | DTOs, entities, and enums for data transfer |
| **exception/** | Global exception handling and custom exceptions |
| **config/** | Spring security and application configuration |
| **resources/** | Application properties and static files |
| **test/** | Unit and integration test classes |
| **target/** | Compiled output, JAR files, and build artifacts |

| File | Description |
|------|-------------|
| `pom.xml` | Maven dependencies and project configuration |
| `QuantityMeasurementAppSpringBootApplication.java` | Spring Boot application entry point |
| `application.properties` | Development environment configuration |
| `application-prod.properties` | Production environment configuration |
| `SecurityConfig.java` | Spring Security configuration (CORS, CSRF, session management) |

#### Development
- Framework: Spring Boot
- Database: H2 (embedded)
- Build Tool: Maven
- API Documentation: Swagger
- Testing: JUnit 5 + Mockito
