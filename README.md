# User Backend Service

**user-backend-service** is a Java/Spring Boot-based backend application providing a production-level API for the `user` entity. This service includes user login functionality with JWT-based authentication and uses H2 as the database.

---

## Features

- **JWT Authentication**: Secure login and session management.
- **Database**: Lightweight, in-memory H2 database for rapid development and testing.
- **Validation**: Input validation for secure and reliable operations.
- **Error Handling**: Centralized exception management for consistent and clear responses.
- **Scalability**: Designed for scalability using Spring Boot's robust framework.

---

## Technologies Used

- **Java**: Version 17 or higher.
- **Spring Boot**: For building RESTful APIs and managing application configuration.
- **JWT**: For secure authentication and authorization.
- **H2 Database**: Lightweight, in-memory database for development.
- **Gradle**: For dependency management and build automation.

---

## Installation

### Prerequisites

- **Java Development Kit (JDK)**: Version 17 or higher.
- **Gradle**: Installed and configured on your system.

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/user-backend-service.git
   ```

2. Navigate to the project directory:
   ```bash
   cd user-backend-service
   ```

3. Build the project:
   ```bash
   gradle clean build
   ```

4. Run the application:
   ```bash
   gradle bootRun
   ```

The service will be available at [http://localhost:8080](http://localhost:8080).

---

## Configuration

The application uses an **H2 database** for development. To access the H2 console:

1. Open [http://localhost:8080/h2-console](http://localhost:8080/h2-console).
2. Use the following credentials:
   - **JDBC URL**: `jdbc:h2:mem:testdb`
   - **Username**: `sa`
   - **Password**: `password`

---

## Project Structure

```
src/
├── main/
│   ├── java/
│   │   ├── controller/       # REST Controllers for API endpoints
│   │   ├── model/            # Entity and Data Transfer Objects (DTOs)
│   │   ├── repository/       # Spring Data JPA repositories
│   │   ├── security/         # JWT and authentication logic
│   │   ├── service/          # Business logic services
│   │   └── utils/            # Utility classes and helpers
│   ├── resources/
│   │   ├── application.properties  # Application configuration
│   │   └── data.sql                # Sample data for H2 database
```

---

## Integration with **user-frontend-service**

For a complete experience, integrate this backend with the **user-frontend-service**, a React-based frontend application. Follow the setup instructions in the frontend's repository and ensure the backend is running before launching the frontend.

### Key Features of the Frontend

- **React**: Built using functional components and hooks.
- **API Integration**: Communicates with this backend service.
- **Reusable Components**: Modular architecture for maintainability.
- **State Management**: Supports Context API.
- **Routing**: Navigation using React Router.

---

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

Enjoy coding and building your projects with the **user-backend-service** and **user-frontend-service**! 😊
