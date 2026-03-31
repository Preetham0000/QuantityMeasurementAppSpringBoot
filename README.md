# Quantity Measurement App - Spring Boot REST API

A Spring Boot-based REST service for performing quantity measurements with support for comparison, conversion, and arithmetic operations with multiple measurement types (Length, Weight, Volume, Temperature).


### API Endpoints
Base URL: http://localhost:8080/api/v1/quantities

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

### Project Structure 
src/
├── main/java/com/app/quantitymeasurement/
│   ├── controller/        # REST controllers
│   ├── service/           # Business logic
│   ├── repository/        # JPA repositories
│   ├── model/             # DTOs and entities
│   ├── exception/         # Exception handling
│   └── config/            # Security & app config
└── resources/
    └── application.properties
