# Blogging Web App

## Overview
This is a Blogging web application built using Spring Boot, REST API, JPA, MySQL, and API testing with Postman. The application provides CRUD operations for managing posts and comments. There are two main controllers: Posts and Comments, each offering functionalities to add, retrieve, update, and delete posts/comments.

## Technologies Used
- Spring Boot
- REST API
- Spring Boot
- JPA (Java Persistence API)
- MySQL
- Postman

## Features
- **Posts Controller:**
  - Create a new post
  - Retrieve all posts
  - Retrieve a specific post by ID
  - Update an existing post
  - Delete a post
  
- **Comments Controller:**
  - Add a comment to a specific post
  - Retrieve all comments for a specific post
  - Retrieve a specific comment by ID
  - Update an existing comment
  - Delete a comment

## Installation
1. **Clone the repository:**
    ```bash
    git clone https://github.com/nikunjpansari/Blogging-Application
    ```
2. **Import project into IDE:**
    - Import the project into your preferred IDE (Eclipse, IntelliJ IDEA, etc.).
3. **Configure MySQL database:**
    - Create a MySQL database named `blog_app`.
    - Update `application.properties` with your database configuration.
4. **Run the application:**
    - Run the `BlogAppApplication.java` class to start the Spring Boot application.

## Usage
- Access the application at `http://localhost:8080`.
- Use Postman or any other API client to interact with the endpoints.
- API documentation can be accessed at `http://localhost:8080/swagger-ui.html`.

## API Documentation

### Posts API:

#### Retrieve all posts
- **Method:** GET
- **URL:** `/api/posts`
- **Description:** Retrieves all posts.

#### Retrieve a specific post by ID
- **Method:** GET
- **URL:** `/api/posts/{id}`
- **Description:** Retrieves a specific post by its ID.

#### Create a new post
- **Method:** POST
- **URL:** `/api/posts`
- **Description:** Creates a new post.

#### Update an existing post
- **Method:** PUT
- **URL:** `/api/posts/{id}`
- **Description:** Updates an existing post identified by its ID.

#### Delete a post
- **Method:** DELETE
- **URL:** `/api/posts/{id}`
- **Description:** Deletes a post identified by its ID.

### Comments API:

#### Retrieve all comments for a specific post
- **Method:** GET
- **URL:** `/api/posts/{postId}/comments`
- **Description:** Retrieves all comments associated with a specific post.

#### Retrieve a specific comment by ID
- **Method:** GET
- **URL:** `/api/posts/{postId}/comments/{commentId}`
- **Description:** Retrieves a specific comment by its ID, associated with a specific post.

#### Add a comment to a specific post
- **Method:** POST
- **URL:** `/api/posts/{postId}/comments`
- **Description:** Adds a new comment to a specific post.

#### Update an existing comment
- **Method:** PUT
- **URL:** `/api/posts/{postId}/comments/{commentId}`
- **Description:** Updates an existing comment identified by its ID, associated with a specific post.

#### Delete a comment
- **Method:** DELETE
- **URL:** `/api/posts/{postId}/comments/{commentId}`
- **Description:** Deletes a comment identified by its ID, associated with a specific post.

## API Testing
- Import the Postman collection provided in the `postman` directory.
- Run the collection to test the API endpoints.

