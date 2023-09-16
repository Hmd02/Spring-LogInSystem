# LogInSystem :gear:

## :warning: Important Note 

Before getting started, please ensure you have the following prerequisites:

- [Spring Tool Suite 4](#) :computer:
- A compatible database for the backend services :floppy_disk:

For the database, no need to create tables manually; the system uses **ORM** :file_folder: (Object-Relational Mapping) for this purpose. By default, this backend uses **PostgreSQL** :elephant:, but you can configure it for another database if necessary. 

To configure the database, follow the steps in the [Configuration](#configuration) section below.

## :information_source: About

Welcome to the LogInSystem! :wave: This backend has been developed using **Spring Boot** :spring: to create APIs. It leverages **ORM** :file_folder: for seamless database interactions and employs regular expressions :1234: for data validation.

## :rocket: Getting Started

To get started with the LogInSystem, follow these steps:

### 1. Prerequisites

- Install [Spring Tool Suite 4](#link-to-installation-guide) on your development machine.

### 2. Database Setup

- Create a database of your choice. Do not worry about creating tables manually; the **ORM** will take care of that.

### 3. Dependencies

- If you decide to use a different database, update the `pom.xml` :notebook: file for each service with the necessary dependencies. Make sure to include the required drivers and libraries.

### 4. Database Configuration

- Configure your database connection in the `application-dev.properties` :wrench: file for each service. You can find this file in the `src/main/resources` :file_folder: directory of each service.

## :gear: Usage

Once you have set up the LogInSystem, you can start utilizing the provided APIs for various login-related tasks.

## :art: Icons Used 

- :computer: - Computer
- :floppy_disk: - Floppy Disk
- :file_folder: - File Folder
- :wrench: - Wrench
- :spring: - Spring Boot
- :notebook: - Notebook
- :elephant: - PostgreSQL
- :1234: - Regular Expressions
- :gear: - Gear

Feel free to explore the code and customize it to suit your specific requirements!
