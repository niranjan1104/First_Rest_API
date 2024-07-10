# RESTful API with Express.js

This repository contains a basic RESTful API implemented using Node.js and Express.js. The API provides endpoints for managing user data stored in a JSON file (`MOCK_DATA.json`). It supports CRUD operations (Create, Read, Update, Delete) for user resources.

## Features

- **GET `/users`**
  - Returns an HTML page listing all user first names.
  
- **GET `/api/users`**
  - Returns a JSON array containing all users.

- **GET `/api/users/filter`**
  - Accepts query parameters (`gender` and `job_title`) to filter users based on specified criteria.
  
- **GET `/api/users/:id`**
  - Retrieves a specific user by ID.
  
- **POST `/api/users`**
  - Adds a new user to the database (`MOCK_DATA.json`) based on data provided in the request body.
  
- **PUT `/api/users/:id`**
  - Updates an existing user specified by ID with new data provided in the request body.
  
- **PATCH `/api/users/:id`**
  - Similar to `PUT`, updates an existing user but allows partial updates based on data provided in the request body.
  
- **DELETE `/api/users/:id`**
  - Deletes a user specified by ID from the database and adjusts the IDs of remaining users accordingly.

## Technologies Used

- Node.js
- Express.js
- JSON file (`MOCK_DATA.json`) for storing user data
- File system (`fs`) module for reading and writing JSON data

