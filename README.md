# ECommerce

## Overview

The `product-catalog-service` is a microservice designed to manage product catalogs. It provides endpoints for handling categories and products, including creating, reading, updating, and deleting them. This service is built using Java and Spring Boot, leveraging Maven for dependency management and Docker for containerization.

## Project Structure

Here's a brief overview of the project's directory structure:

- `.idea/` - IntelliJ IDEA project files (IDE-specific).
- `.mvn/` - Maven wrapper files.
- `src/` - Source code for the application.
    - `main/`
        - `java/`
            - `productcatalogservice/`
                - `controller/` - Contains REST controllers for categories and products.
                    - `CategoryController.java` - Controller for category-related endpoints.
                    - `ProductController.java` - Controller for product-related endpoints.
                - `dto/` - Data Transfer Objects for communication.
                - `entity/` - JPA entities for database interaction.
                    - `CategoryEntity.java` - Entity representing a category.
                    - `ProductEntity.java` - Entity representing a product.
                - `repository/` - Spring Data JPA repositories.
                    - `CategoryRepository.java` - Repository for category entities.
                    - `ProductRepository.java` - Repository for product entities.
                - `service/` - Service layer for business logic.
                    - `impl/`
                        - `CategoryServiceImpl.java` - Implementation of category service.
                        - `ProductServiceImpl.java` - Implementation of product service.
                    - `ICategoryService.java` - Interface for category service.
                    - `IProductService.java` - Interface for product service.
                - `ProductCatalogServiceApplication.java` - Main application class.
        - `resources/`
            - `static/` - Static resources (e.g., JavaScript, CSS).
            - `templates/` - Templates for rendering views.
            - `application.properties` - Application configuration properties.
- `target/` - Compiled bytecode and build artifacts.
- `.dockerignore` - Specifies files and directories to ignore during Docker build.
- `.gitignore` - Specifies files and directories to ignore in version control.
- `docker-compose.yml` - Docker Compose configuration for multi-container applications.
- `DockerFile` - Dockerfile for building the application image.
- `HELP.md` - Additional help and information about the project.
- `mvnw` - Maven wrapper script (Unix).
- `mvnw.cmd` - Maven wrapper script (Windows).
- `pom.xml` - Maven project configuration file.

## Getting Started

### Prerequisites

- [JDK 11 or higher](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Mav

## Configuration 
- The application configuration can be adjusted in src/main/resources/application.properties

## Endpoints

## Categories:

- GET /categories - List all categories
- POST /categories - Create a new category 
- GET /categories/{id} - Retrieve a category by ID 
- PUT /categories/{id} - Update a category by ID 
- DELETE /categories/{id} - Delete a category by ID
 ## Products:

- GET /products - List all products 
- POST /products - Create a new product 
- GET /products/{id} - Retrieve a product by ID 
- PUT /products/{id} - Update a product by ID 
- DELETE /products/{id} - Delete a product by ID
