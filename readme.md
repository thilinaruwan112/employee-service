# Employee Service

## Description
The Employee Service is a part of a Spring Boot application that manages employee-related functionality such as adding, updating, deleting, and fetching employee details. It is built using Java, Spring Boot, and integrates with a MySQL database.

## Features
- Add an employee
- Retrieve employee details
- Update employee information
- Delete an employee

## Technologies Used
- **Spring Boot**: For building the REST API and backend logic.
- **JPA (Java Persistence API)**: For interacting with the MySQL database.
- **Lombok**: For reducing boilerplate code.
- **Maven**: For managing dependencies and building the project.

## Getting Started

### Prerequisites
- Java 17 or later
- Maven
- MySQL (or H2 for in-memory database)

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/employee-service.git
   ```

2. Navigate to the project directory:
   ```bash
   cd employee-service
   ```

3. Update the `application.properties` or `application.yml` to configure the database connection if using MySQL:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```

4. Install dependencies and run the application:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

## Endpoints

* **POST** `/employees` - Create a new employee
  * Request Body:
    ```json
    {
        "name": "John Doe",
        "age": 30,
        "departmentId": 1
    }
    ```
* **GET** `/employees/{id}` - Get employee details by ID
* **PUT** `/employees/{id}` - Update employee details by ID
* **DELETE** `/employees/{id}` - Delete employee by ID

## License
This project is licensed under the MIT License - see the LICENSE file for details.
