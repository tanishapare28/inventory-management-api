
# Inventory Management REST API

## Project Description
This is a backend Inventory Management REST API developed using Java, Spring Boot, Spring Data JPA, and MySQL.

The application allows users to add, view, update, and delete products.

## Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA and Hibernate
- MySQL
- Maven
- REST API

## Features
- Add a new product
- View all products
- View a product by ID
- Update product details
- Delete a product
- Validate product name, price, and quantity
- Connect to a MySQL database

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/products` | Get all products |
| GET | `/api/products/{id}` | Get product by ID |
| POST | `/api/products` | Add a product |
| PUT | `/api/products/{id}` | Update a product |
| DELETE | `/api/products/{id}` | Delete a product |

## How to Run the Project

1. Install Java 17 and MySQL.
2. Configure the database settings in `src/main/resources/application.properties`.
3. Open a terminal in the project folder.
4. Run the following command:

```powershell
.\mvnw.cmd spring-boot:run
```

5. The API runs at `http://localhost:8080`.

## Build the Project

Run this command to package the application:

```powershell
.\mvnw.cmd clean package
```

## Validation
The API was manually tested for valid product creation, empty product names, negative prices, negative quantities, and requests using invalid product IDs.
