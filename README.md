# E-commerce Website

A full-stack e-commerce platform built with Angular and Spring Boot.

## Overview

This E-Commerce website is a full-stack application built with Angular and Java Spring Boot. It includes a wide range of features and functionalities necessary for a modern online store. The project is designed to showcase best practices in building robust and secure web applications using the technologies mentioned above.

## Project Structure

- `frontend/` - Angular 14 application
- `backend/` - Spring Boot application

## Features

- **User Authentication**: Utilizes Spring Security and Okta for secure user authentication and authorization.

- **Product Catalog**: Allows users to browse and search for products with a well-structured product catalog.

- **Shopping Cart**: Users can add products to their cart and proceed to checkout seamlessly.

- **Payment Integration**: Integration with Stripe for handling payments.

- **Swagger API Documentation**: Detailed API documentation using Swagger.

- **Responsive Design**: Improved styling and responsive design for a better user experience.

- **Frontend Hosting**: The frontend is hosted on Netlify for easy access.

- **Backend Hosting**: The backend is hosted on Render.

- **Database Hosting**: The database is hosted on Railway.

### Frontend (Angular 14)
- Modern, responsive UI built with Angular 14
- User authentication with Okta
- Product catalog with categories
- Shopping cart functionality
- Secure checkout with Stripe integration
- Order history and tracking

### Backend (Spring Boot)
- RESTful API services
- User authentication and authorization
- Product management
- Order processing
- Database integration
- Security configurations

## Prerequisites

- Node.js (v14 or higher)
- Angular CLI (v14)
- Java JDK 17 or later
- Maven 3.6.3 or later
- MySQL/PostgreSQL (or your preferred database)

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```
   The application will be available at `https://localhost:4200`

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run the application:
   ```bash
   mvn spring-boot:run
   ```
   The API will be available at `http://localhost:8080`

## Environment Variables

Create a `.env` file in the root of both frontend and backend directories with the following variables:

### Frontend (.env)
```
API_URL=http://localhost:8080/api
OKTA_CLIENT_ID=your_okta_client_id
OKTA_ISSUER_URI=your_okta_issuer_uri
STRIPE_PUBLIC_KEY=your_stripe_public_key
```

### Backend (application.properties)
```
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
spring.datasource.username=db_username
spring.datasource.password=db_password
spring.jpa.hibernate.ddl-auto=update

# JWT Configuration
jwt.secret=your_jwt_secret
jwt.expiration=86400000

# Stripe Configuration
stripe.secret.key=your_stripe_secret_key
```

## Development

### Running Tests

#### Frontend
```bash
cd frontend
ng test
```

#### Backend
```bash
cd backend
mvn test
```

### Building for Production

#### Frontend
```bash
cd frontend
ng build --configuration production
```

#### Backend
```bash
cd backend
mvn clean package -DskipTests
```

## Technologies Used

### Frontend
- Angular 14
- TypeScript
- Bootstrap 5
- Okta for authentication
- Stripe for payments
- RxJS for state management

### Backend
- Spring Boot
- Spring Security
- Spring Data JPA
- JWT Authentication
- Maven
- MySQL/PostgreSQL

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please open an issue in the repository or contact the development team.

## Acknowledgments

- [Angular](https://angular.io/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Okta](https://www.okta.com/)
- [Stripe](https://stripe.com/)
- [Bootstrap](https://getbootstrap.com/)
