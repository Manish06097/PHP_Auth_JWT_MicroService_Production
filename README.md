# JWT Authentication Microservices with Laravel 10 and PHP 8

This repository contains a microservices project built using Laravel 10 and PHP 8, implementing JWT (JSON Web Tokens) authentication. It also includes documentation generated with L5 Swagger for easier API exploration. This README will guide you through the installation process, setup of the project, how to test the services, and encourage you to contribute to the project.

## Installation

Follow these steps to set up and run the microservices project:

### Prerequisites

Before you begin, ensure you have the following prerequisites installed on your system:

- [PHP](https://www.php.net/) 8 or higher
- [Composer](https://getcomposer.org/)
- [Node.js](https://nodejs.org/)
- [NPM](https://www.npmjs.com/) (Node Package Manager)

### Clone the Repository

First, clone this GitHub repository to your local machine:

```bash
git clone https://github.com/Manish06097/PHP_Auth_JWT_MicroService_Production.git
```


#### Install Dependencies
Navigate to the project's root directory and install the PHP and JavaScript dependencies:

```bash
cd PHP_Auth_JWT_MicroService_Production
composer install
```

#### Configure JWT Authentication
To set up JWT authentication, follow these steps:
1. Open the .env file and configure your database settings:
   ```bash
    DB_CONNECTION=mysql
    DB_HOST=your-database-host
    DB_PORT=your-database-port
    DB_DATABASE=your-database-name
    DB_USERNAME=your-database-username
    DB_PASSWORD=your-database-password
   ```
2. Generate a JWT secret key:
   ```bash
   php artisan jwt:secret
   ```

#### Migrate the Database
Run the database migrations to create the necessary tables
```bash
php artisan migrate
```

#### Generate Swagger Documentation
To generate Swagger documentation for your APIs, use the following command:
```bash
php artisan l5-swagger:generate
```

#### Running the Microservices
You can now run your microservices. Start the Laravel development server:

```bash
php artisan serve
```

Your microservices should now be up and running. You can access the Swagger documentation at http://localhost:8000/api/documentation.

### Testing the Services

#### Automated Testing
To run automated tests, execute the following command:

```bash
php artisan test
```
This command will run the test suite and provide you with feedback on the functionality and reliability of your microservices.

## Contribute and Show Your Support
If you find this project useful and like what you see, please consider giving it a star on GitHub. Your support encourages the maintainers and lets them know that you appreciate their work.
If you encounter issues or have suggestions for improvements, please don't hesitate to raise issues on the project's GitHub repository. You're also welcome to contribute by submitting pull requests with enhancements or bug fixes. Your contributions will help make this project even better for the community.
Thank you for your interest in and support of this microservices project!
