# LogInSystem Backend

This repository contains the backend system for user authentication and password management using Spring Boot and PostgreSQL. It offers APIs for user signup, login, and password reset.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Technologies Used](#technologies-used)
- [API Endpoints](#api-endpoints)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before using this backend, ensure you have the following:

1. [Spring Tool Suite 4](https://spring.io/tools) or a compatible Java IDE.
2. PostgreSQL installed and running.
3. Knowledge of how to configure a database in Spring Boot applications.

## Technologies Used

- **Spring Boot**: A powerful framework for building Java-based applications.
- **Regular Expression**: Used for pattern matching and validation.
- **PostgreSQL**: A popular open-source relational database.
- **Object-Relational Mapping (ORM)**: Simplifies database interactions with Java objects.
    <table align="center">
    <tr><th colspan="4">
    Technologies
    </th>
    </tr>
    <tr>
    <td>
    <img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="Spring Boot" width="50"></td>
    <td><img src="https://cdn0.iconfinder.com/data/icons/programming-and-coding-3/48/16-Code-1024.png" width="50"></td>
    <td><img src="https://www.vectorlogo.zone/logos/postgresql/postgresql-icon.svg" alt="PostgreSQL" width="50"></td>
    <td><img src="https://cdn3.iconfinder.com/data/icons/human-resources-70/133/12-1024.png" width="50"></td>
    </tr>
    </table>

## API Endpoints

1. **User Signup**
   - Endpoint: `http://localhost:8085/signup`
   - Method: POST
   - Input:
     ```json
     {
         "userId": "newUserID",
         "dob": "16/2/22",
         "name": "Name Of user",
         "password": "password"
     }
     ```

2. **User Login**
   - Endpoint: `http://localhost:8085/login/{userId}/{password}`
   - Method: GET

3. **Password Reset (Step 1 - Check User)**
   - Endpoint: `http://localhost:8085/resetIn`
   - Method: POST
   - Input:
     ```json
     {
         "userId": "UserID",
         "dob": "16/2/22"
     }
     ```

4. **Password Reset (Step 2 - Update Password)**
   - Endpoint: `http://localhost:8085/updatePassword/{userID}/{newpassword}`
   - Method: POST

Explore the application for additional APIs that may assist in your UI development.

## Setup

1. Clone this repository to your local machine.

2. Configure your PostgreSQL database in `application-dev.properties` located in `src/main/resources`.

3. Ensure you have the necessary dependencies added in the `pom.xml` file for each service if you want to use a different database.

## Usage

To use this backend, start the Spring Boot application and make HTTP requests to the provided API endpoints. You can test the APIs using tools like [Postman](https://www.postman.com/).

## Contributing

Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please feel free to open an issue or create a pull request.

