# Rest-API using Go, GORM, and GoFr

Welcome to the Rest-API built with Go (Golang), and GoFr framework for accelerating micro-service development.

## Introduction

This project demonstrates the creation of a RESTful API utilizing the Go programming language, GORM for database handling, and GoFr, an Opinionated Go Framework. These technologies combined provide an efficient, scalable, and maintainable way to develop web applications and microservices.

### Technologies Used

- **Go (Golang):**
  Go is a powerful, efficient, and easy-to-learn programming language that enables the development of fast and scalable applications. It's renowned for its simplicity and concurrency support.

- **GORM:**
  GORM, an Object-Relational Mapping (ORM) framework, simplifies interactions between Go objects and relational databases. It abstracts complex database operations, allowing developers to focus on building the application logic.

- **GoFr:**
  GoFr is an Opinionated Web Framework written in Go. It streamlines the development process by emphasizing simplicity and offering tools to create robust and scalable applications.

## Prerequisites

Before starting with this project, ensure you have the following prerequisites set up:

1. **Go Installation:**
   Install Go (Golang) by following the official installation instructions [here](https://golang.org/doc/install).

2. **GoFr:**
   Install GoFr using the following command: go get gofr.dev

3. **Docker:**
Consider using Docker with a SQL image for database management. The project uses a MySQL Docker image; you can find the official MySQL Docker image [here](https://hub.docker.com/_/mysql).

## Project Structure

The project follows a layered architecture approach for enhanced maintainability and scalability:
![image](https://github.com/prakhar12330/gofr_REST_API/assets/84180549/b8b400ff-3e65-494a-9488-67a30e890dcf)


- **Configs:** Directory for configuration files.
- **Handler:** Contains request handling logic.
- **Model:** Defines the data models.
- **Datastore:** Manages database interactions.
- **main.go:** Entry point orchestrating the project.

## GORM and GoFr Integration

GoFr seamlessly integrates with GORM, making database management efficient and straightforward. It provides configurations to manage various datastores like PostgreSQL, Redis, MongoDB, SQL, and Cassandra. This project utilizes GORM via GoFr for database operations.

### Example Configuration

To connect to a MySQL database, define the configuration in the `configs/.env` file:
![image](https://github.com/prakhar12330/gofr_REST_API/assets/84180549/b1d5e2bb-fc55-4550-8b31-31293cd81b48)


## Getting Started

### Running the Application

1. **Setup MySQL Docker Image:**
   Run the following command to set up the MySQL Docker image: docker run --name gofr-mysql -e MYSQL_ROOT_PASSWORD=password -p 2001:3306 -d mysql

2. **Launch the API:**
   Execute the `main.go` file to start the REST API: go run main.go


Upon running, you'll see informative logs confirming the server's startup and database connection establishment. The API is ready to receive requests.

## Contributors

This project is maintained by Prakhar Singh.








