# JAX-RS Spring Boot Application

This project is a simple banking service built with Spring Boot and JAX-RS (Jersey) to provide a RESTful API for managing bank accounts. It uses an in-memory H2 database for data storage and supports both JSON and XML data formats.

## Technologies Used

*   **Spring Boot:** For easy setup and configuration of the application.
*   **Spring Data JPA:** To interact with the database.
*   **JAX-RS (Jersey):** For creating the RESTful web services.
*   **Hibernate:** As the JPA implementation.
*   **H2 Database:** An in-memory database for development and testing.
*   **Maven:** For project build and dependency management.
*   **Lombok:** To reduce boilerplate code.
*   **JAXB:** For XML data binding.

## Features

*   **CRUD Operations:** Create, Read, Update, and Delete bank accounts.
*   **RESTful API:** Exposes endpoints for managing accounts.
*   **Dual-Format Support:** The API can consume and produce both JSON and XML.
*   **In-Memory Database:** No external database setup is required.

## API Endpoints

The base path for all endpoints is `/banque`.

| Method | Path              | Description                                  | Consumes/Produces                |
|--------|-------------------|----------------------------------------------|----------------------------------|
| `GET`    | `/comptes`        | Retrieves a list of all bank accounts.       | JSON, XML                        |
| `GET`    | `/comptes/{id}`   | Retrieves a specific account by its ID.      | JSON, XML                        |
| `POST`   | `/comptes`        | Creates a new bank account.                  | JSON, XML                        |
| `PUT`    | `/comptes/{id}`   | Updates an existing bank account by its ID.  | JSON, XML                        |
| `DELETE` | `/comptes/{id}`   | Deletes a bank account by its ID.            | JSON, XML                        |

## Getting Started

### Prerequisites

*   Java Development Kit (JDK) 17 or later.
*   Apache Maven.

### Running the Application

1.  **Clone the repository:**
    ```sh
    git clone <https://github.com/Yasineert/TP-7-JAXRS--Jersey/edit/main>
    cd jaxrs
    ```

2.  **Build and run the application using Maven:**
    ```sh
    mvn spring-boot:run
    ```

The application will start on port `8082`.

## Database Configuration

The application uses an in-memory H2 database. You can access the H2 console in your browser at:

[http://localhost:8082/h2-console](http://localhost:8082/h2-console)

Use the following credentials to log in:

*   **JDBC URL:** `jdbc:h2:mem:banque`
*   **User Name:** `sa`
*   **Password:** (leave blank)


<img width="807" height="464" alt="Screenshot 2025-11-15 163034" src="https://github.com/user-attachments/assets/143d7202-1c0a-4c94-9827-8e85278d574c" />
