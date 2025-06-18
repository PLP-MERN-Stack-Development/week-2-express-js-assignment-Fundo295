[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19777092&assignment_repo_type=AssignmentRepo)
# Express.js RESTful API Assignment

This assignment focuses on building a RESTful API using Express.js, implementing proper routing, middleware, and error handling.

## Assignment Overview

You will:
1. Set up an Express.js server
2. Create RESTful API routes for a product resource
3. Implement custom middleware for logging, authentication, and validation
4. Add comprehensive error handling
5. Develop advanced features like filtering, pagination, and search

## Getting Started

1. Accept the GitHub Classroom assignment invitation
2. Clone your personal repository that was created by GitHub Classroom
3. Install dependencies:
   ```
   npm install
   ```
4. Run the server:
   ```
   npm start
   ```

## Files Included

- `Week2-Assignment.md`: Detailed assignment instructions
- `server.js`: Starter Express.js server file
- `.env.example`: Example environment variables file

## Requirements

- Node.js (v18 or higher)
- npm or yarn
- Postman, Insomnia, or curl for API testing

## API Endpoints

The API will have the following endpoints:

- `GET /api/products`: Get all products
- `GET /api/products/:id`: Get a specific product
- `POST /api/products`: Create a new product
- `PUT /api/products/:id`: Update a product
- `DELETE /api/products/:id`: Delete a product

## Submission

Your work will be automatically submitted when you push to your GitHub Classroom repository. Make sure to:

1. Complete all the required API endpoints
2. Implement the middleware and error handling
3. Document your API in the README.md
4. Include examples of requests and responses

## Resources

- [Express.js Documentation](https://expressjs.com/)
- [RESTful API Design Best Practices](https://restfulapi.net/)
- [HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

# 🛍️ Product RESTful API with Express.js

This project is a simple RESTful API built with **Express.js** that manages a list of products. It supports full CRUD operations, middleware for logging, authentication, and validation, and includes advanced features such as filtering, pagination, and product search.

---

## 🚀 Features

- ✅ Full CRUD functionality
- 🧱 Middleware implementation:
  - Request logger
  - JSON body parser
  - API key authentication
  - Input validation
- 🧰 Error handling with custom error classes
- 🔍 Filtering by category
- 🔢 Pagination support
- 🔎 Search by name
- 📊 Product statistics

---

🧪 API Endpoints
🟢 GET /api/products
Get all products with optional filters:

category (e.g. /api/products?category=electronics)

page and limit for pagination

## 🔵 GET /api/products/:id
Get a product by ID

## 🟡 POST /api/products
Create a new product (requires API key in x-api-key header)

json
Copy
Edit
{
  "name": "TV",
  "description": "55 inch OLED",
  "price": 999.99,
  "category": "electronics",
  "inStock": true
}
## 🟠 PUT /api/products/:id
Update an existing product (requires API key)

## 🔴 DELETE /api/products/:id
Delete a product by ID (requires API key)

## 🔐 Authentication
For POST, PUT, and DELETE requests, include the following header:

http
Copy
Edit
x-api-key: mysecretkey
📊 Stats (Optional Feature)
Future endpoint ideas:

/api/products/stats — Return total product count, and count per category

## 🛠 Tech Stack
Node.js

Express.js

UUID

Body-parser

## Run the server 
node server.js

