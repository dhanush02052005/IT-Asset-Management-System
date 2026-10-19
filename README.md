# IT Asset Management System

## 📌 Project Overview

The **IT Asset Management System** is a web-based application developed to manage and track IT assets efficiently within an organization. The system helps maintain asset records, monitor asset details, and organize asset-related information through a structured application.

The project is developed using Java and Spring Boot for backend development, with a database for persistent storage. It demonstrates core concepts of enterprise application development, including REST APIs, dependency injection, layered architecture, and database integration.

## 🎯 Objectives

- Maintain centralized records of IT assets.
- Simplify asset tracking and management.
- Perform CRUD (Create, Read, Update, Delete) operations on asset records.
- Improve the organization and accessibility of asset information.
- Integrate the application with a relational database.
- Apply Spring Boot concepts to develop a maintainable backend application.

## ✨ Key Features

- **Asset Registration:** Add new IT asset records.
- **Asset Management:** View and maintain asset information.
- **Asset Updates:** Modify existing asset details.
- **Asset Deletion:** Remove asset records when required.
- **REST API Integration:** Expose endpoints to perform asset-related operations.
- **Database Integration:** Store and retrieve asset information from the configured database.
- **Layered Architecture:** Separate controller, service, and repository responsibilities.
- **Exception Handling:** Handle application errors where implemented.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Java |
| Backend Framework | Spring Boot |
| API Development | Spring Web, REST APIs |
| Data Access | Spring Data JPA |
| ORM | Hibernate |
| Database | MySQL / H2, depending on configuration |
| Build Tool | Maven |
| Testing | JUnit / Mockito, if configured |
| Version Control | Git, GitHub |

## 🏗️ Application Architecture

The application follows a layered architecture to separate responsibilities and improve maintainability.

- **Controller Layer:** Handles HTTP requests and sends responses to the client.
- **Service Layer:** Contains business logic and coordinates application operations.
- **Repository Layer:** Uses Spring Data JPA to access and manage database records.
- **Entity Layer:** Represents the asset data stored in the database.
- **Database Layer:** Persists asset information using the configured database.

## 🔄 Application Workflow

1. The client sends an HTTP request to the application.
2. The controller receives the request through the appropriate REST endpoint.
3. The controller calls the service layer to perform the required operation.
4. The service layer applies business logic and interacts with the repository.
5. The repository communicates with the database using Spring Data JPA and Hibernate.
6. The database returns the requested information or confirms the data modification.
7. The service and controller process the result.
8. The application returns an appropriate HTTP response to the client.

## ⚙️ Prerequisites

Install the following software before running the project:

- Java Development Kit (JDK)
- Maven
- MySQL Server, if using MySQL configuration
- Git
- An IDE such as IntelliJ IDEA, Eclipse, or Visual Studio Code

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_PROJECT_FOLDER>
```

Replace the placeholders with your actual repository URL and project directory.

### 2. Configure the Database

For MySQL, update the `application.properties` file with your database details.

```properties
server.port=8088

spring.datasource.url=jdbc:mysql://localhost:3306/materialdb?createDatabaseIfNotExist=true&useSSL=false&serverTimezone=UTC
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Use the database name, port, and credentials specified by your project. If the project is configured to use H2, select the corresponding H2 profile or configuration instead.

### 3. Build the Application

Open a terminal in the project root directory and run:

```bash
mvn clean install
```

This command compiles the application, resolves dependencies, and runs the configured tests.

### 4. Run the Application

Start the Spring Boot application using:

```bash
mvn spring-boot:run
```

Alternatively, run the main Spring Boot application class from your IDE.

### 5. Test the REST APIs

Use Postman or another HTTP client to test the asset management endpoints.

Typical operations include:

- `POST` — Create an asset.
- `GET` — Retrieve asset information.
- `PUT` — Update an existing asset.
- `DELETE` — Delete an asset.

Use the actual endpoint paths and request formats defined in the project.

## 🧪 Testing

The application can be tested by verifying:

- Asset creation and retrieval.
- Updating existing asset information.
- Deleting asset records.
- Database connectivity and persistence.
- REST API responses and error handling.
- Validation and exception handling, where implemented.

## 📚 Concepts Demonstrated

- Object-Oriented Programming in Java.
- Spring Boot application development.
- Dependency Injection and Inversion of Control.
- RESTful web service development.
- Spring Data JPA and Hibernate.
- CRUD operations.
- Layered application architecture.
- Database configuration and integration.
- Maven-based project management.

## 🔮 Future Enhancements

- Add user authentication and role-based access control.
- Track asset allocation and return history.
- Introduce asset maintenance and warranty reminders.
- Add search, filtering, and reporting features.
- Implement audit logs for asset modifications.
- Develop a dedicated frontend dashboard.

## 👨‍💻 Project Information

**Project Name:** IT Asset Management System

**Project Type:** HON (Hands-on) Project

**Domain:** IT Asset Management

**Primary Technology:** Java, Spring Boot, Spring Data JPA

## 📄 License

This project is intended for educational and demonstration purposes. Add an appropriate open-source license if you intend to distribute the project publicly.
