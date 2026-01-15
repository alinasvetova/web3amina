# Assignment 3: Building a CRUD API with Node.js and MongoDB

## Project Overview
[cite_start]This repository contains the implementation of a fully functional CRUD (Create, Read, Update, Delete) API for a simple blogging platform, as required by Assignment 3[cite: 1, 3]. The project utilizes Node.js and Express for the server-side architecture and MongoDB (Atlas) for data persistence. [cite_start]A client-side interface is included to demonstrate the API functionality[cite: 35].

## Technology Stack
* **Runtime Environment:** Node.js
* **Web Framework:** Express.js
* **Database:** MongoDB Atlas (Cloud)
* **Object Modeling:** Mongoose
* **Frontend:** HTML5, CSS3, JavaScript (Fetch API)

## Installation and Setup

### Prerequisites
* Node.js (v14 or higher)
* npm (Node Package Manager)

### Steps to Run
1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <project-directory>
    ```

2.  **Install dependencies:**
    Execute the following command to install required packages (express, mongoose, cors, body-parser):
    ```bash
    npm install
    ```

3.  **Start the server:**
    ```bash
    node server.js
    ```

4.  **Access the application:**
    The server listens on port 3000. Open a web browser and navigate to:
    `http://localhost:3000`

## API Documentation
[cite_start]The application implements the following RESTful endpoints [cite: 10-15]:

| HTTP Method | Endpoint       | Description                                      |
|:------------|:---------------|:-------------------------------------------------|
| **POST** | `/blogs`       | Creates a new blog post.                         |
| **GET** | `/blogs`       | Retrieves a list of all blog posts.              |
| **GET** | `/blogs/:id`   | Retrieves a specific blog post by its unique ID. |
| **PUT** | `/blogs/:id`   | Updates an existing blog post by its unique ID.  |
| **DELETE** | `/blogs/:id`   | Deletes a blog post by its unique ID.            |

## Database Schema
[cite_start]The data model for a blog post complies with the assignment requirements and includes the following fields [cite: 19-23]:

* **title** (String, Required): The title of the blog post.
* **body** (String, Required): The main content of the post.
* **author** (String, Optional): The name of the author. Defaults to "Anonymous" if not provided.
* **createdAt** (Date): Automatically generated timestamp.
* **updatedAt** (Date): Automatically generated timestamp.

## Project Structure
* `server.js`: The entry point of the application. Handles database connection, middleware configuration, and API route definitions.
* `public/index.html`: The frontend interface for interacting with the API.
* `package.json`: Manifest file containing metadata and dependencies.