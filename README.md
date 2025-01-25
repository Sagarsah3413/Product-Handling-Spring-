
# ProdTrack

ProdTrack is a Spring Boot-based application designed to manage product inventories efficiently. The system supports core functionalities such as CRUD operations, image handling, keyword-based product searches, and robust error handling. Initially built with an H2 in-memory database for quick prototyping, the project is in progress to migrate to PostgreSQL for production-grade scalability. JWT-based authentication and authorization are also being integrated to enhance security.
## Features

- CRUD Operations : Add, update, delete, and fetch product details.
- Image Handling: Upload and retrieve product images seamlessly using MultipartFile.
- Search Functionality: Keyword-based search for easy product discovery.
- Database Support:

        1. Initial setup: H2 in-memory database.
        2.  Planned migration: PostgreSQL for better scalability and reliability.

- Authentication: Integration of JWT for secure authentication and authorization (in progress).

- Spring Boot: Utilized for creating RESTful APIs and efficient backend logic.


## API ENDPoints

Product Endpoints

GET `/products`: Fetch all products.

POST `/product`: Add a new product (supports image upload).

GET `/product/{id}`: Fetch product details by ID.

GET `/product/{id}/image`: Retrieve the image of a product.

PUT `/product/{id}`: Update product details and image.

DELETE `/product/{id}`: Delete a product by ID.

GET `/products/search?keyword={keyword}`: Search products by keyword.


## Technologies Used 

- Backend: Spring Boot

- Database: H2 (in-memory), PostgreSQL (planned migration)

- ORM: Hibernate

- Authentication: JWT (in progress)

- Tools: IntelliJ IDEA, Postman, GitHub
## Getting Started

# Prerequisites
- JDK 8 or later
- Maven
- PostgreSQL (for production setup)

# Setup Instructions
1. Clone the repository:
  
         git clone https://github.com/Sagarsah3413/Product-Handling-Spring-.git

4. H2 Database (Default)
The application is pre-configured to use H2 for development:

        spring.datasource.url=jdbc:h2:mem:sagar
        spring.datasource.driverClassName=org.h2.Driver
        spring.jpa.hibernate.ddl-auto=update
        spring.jpa.show-sql=true`

5. PostgreSQL (Planned Production)
   
Update application.properties to configure PostgreSQL:

      spring.datasource.url=jdbc:postgresql://localhost:5432/springBoot
      spring.datasource.username=postgres
      spring.datasource.password=password
      spring.jpa.hibernate.ddl-auto=update
      spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
## Future Enhancements  

JWT Integration: Secure APIs with token-based authentication and role-based access control.

Advanced Filtering: Add sorting and filtering options for product search.

Deployment: Deploy the application to cloud platforms like AWS or Heroku.


## Support

For support, email sahs82341@gmail.com 

