# Blog CRUD API (Assignment 3)

## Description
This project is a CRUD (Create, Read, Update, Delete) API for a simple blogging platform.
It is built using Node.js, Express, and MongoDB. A basic frontend interface is included
to interact with the API.

This project was developed as part of Assignment 3 (Back End).

## Technologies Used
- Node.js
- Express.js
- MongoDB
- Mongoose
- dotenv
- cors
- HTML

## Project Structure
blog-crud-api/
├── server.js
├── package.json
├── .env
├── models/
│   └── Blog.js
├── routes/
│   └── blogRoutes.js
└── public/
    └── index.html

## Installation and Setup

1. Install dependencies
npm install

2. Create .env file
MONGO_URI=mongodb://127.0.0.1:27017/blogdb
PORT=3000

3. Run the server
npm start

The server will run at http://localhost:3000

## API Endpoints

Create a blog post  
POST /blogs  
Request body:
{
  "title": "My Blog",
  "body": "This is the blog content",
  "author": "John Doe"
}

Get all blog posts  
GET /blogs

Get a single blog post  
GET /blogs/:id

Update a blog post  
PUT /blogs/:id  
Request body:
{
  "title": "Updated title",
  "body": "Updated body"
}

Delete a blog post  
DELETE /blogs/:id

## Data Validation
- Title is required
- Body is required
- Author is optional (default: Anonymous)
- Automatic timestamps (createdAt, updatedAt)

## Error Handling
- Handles invalid requests
- Handles invalid MongoDB IDs
- Returns appropriate HTTP status codes
- Returns clear JSON error messages

## Testing
The API was tested manually using Postman.
All CRUD operations (POST, GET, PUT, DELETE) work correctly.

## Frontend
A simple HTML interface is available at http://localhost:3000
It allows creating and viewing blog posts.

## Submission
The project can be submitted as a GitHub repository link
or as a ZIP archive containing all project files.

## Author
Student Name: __________  
Assignment: Assignment 3 – CRUD API
