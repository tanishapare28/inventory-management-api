
# Inventory Management REST API

A backend RESTful API for managing inventory products, developed using Java, Spring Boot, Spring Data JPA, Hibernate, and MySQL.

This project demonstrates CRUD operations, database integration, and input validation in a Spring Boot application.

## Features

- Create a new product
- Retrieve all products
- Retrieve a product by ID
- Update existing product details
- Delete a product
- Validate product names, prices, and quantities
- Integrate with a MySQL database
- Handle requests for products that do not exist

## Technologies Used

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- Hibernate
- MySQL
- Maven
- Bean Validation

## API Endpoints

| HTTP Method | Endpoint | Description |
|---|---|---|
| GET | `/api/products` | Retrieve all products |
| GET | `/api/products/{id}` | Retrieve a product by ID |
| POST | `/api/products` | Create a new product |
| PUT | `/api/products/{id}` | Update an existing product |
| DELETE | `/api/products/{id}` | Delete a product |

## Example Request

Create a product using a `POST` request to `/api/products`.

**Request body:**

```json
{
  "name": "Notebook",
  "price": 50,
  "quantity": 10
}
```

## Prerequisites

- Java JDK
- MySQL Server
- A MySQL database named `inventory_db`

## Database Configuration

Configure your local database connection in:

`src/main/resources/application.properties`

Keep your database credentials private. Do not upload passwords or other secrets to GitHub.

## How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/tanishapare28/inventory-management-api.git
   ```

2. Open the project directory:

   ```bash
   cd inventory-management-api/inventory
   ```

3. Configure the MySQL connection and ensure the `inventory_db` database exists.

4. Start the application on Windows:

   ```powershell
   .\mvnw.cmd spring-boot:run
   ```

5. Access the API at:

   `http://localhost:8080/api/products`

## Build the Project

To build the application using Maven Wrapper:

```powershell
.\mvnw.cmd clean package
```

## Validation and Testing

The API has been manually tested for:

- Successful product creation
- Empty product names
- Negative prices
- Negative quantities
- Requests using invalid product IDs

## Project Purpose

This project demonstrates backend development concepts, RESTful API design, CRUD operations, database integration, and input validation using the Java Spring Boot ecosystem.
