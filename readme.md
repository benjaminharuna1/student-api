# Student Simple Crud API

This is a simple RESTful API CRUD application built with **Node.js**, **Express.js**, and **MongoDB**. The API allows managing student records with CRUD (Create, Read, Update, Delete) operations.

## Features
- Connects to MongoDB using **Mongoose**
- RESTful routes for managing student records
- Uses **dotenv** to load environment variables
- JSON-based request and response handling

## Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or later)
- [MongoDB](https://www.mongodb.com/) (Local or Cloud Atlas)

## Installation
1. **Clone the repository**:
   ```sh
   git clone https://github.com/benjaminharuna1/student-api.git
   cd student-api
   ```
2. **Install dependencies**:
   ```sh
   npm install
   ```
3. **Set up environment variables**:
   - Create a `.env` file in the project root
   - Add the following variables:
     ```env
     PORT=3000
     MONGODB_URI=mongodb+srv://your-username:your-password@your-cluster.mongodb.net/your-database?retryWrites=true&w=majority
     ```
   - Replace `your-username`, `your-password`, and `your-database` with your actual MongoDB credentials.

## Running the Server
Start the server using:
```sh
node server.js
```
OR (if using **nodemon** for auto-restart):
```sh
npx nodemon server.js
```

## API Endpoints
| Method | Endpoint         | Description              |
|--------|----------------|--------------------------|
| GET    | `/students`     | Get all students        |
| GET    | `/students/:id` | Get a student by ID     |
| POST   | `/students`     | Create a new student    |
| PUT    | `/students/:id` | Update a student        |
| DELETE | `/students/:id` | Delete a student        |


## Note:
# To run your post requests use raw json requests from postman

## Troubleshooting
If MongoDB connection fails:
- Ensure `.env` file is correctly configured
- Check if MongoDB service is running
- Restart the server after changes: `Ctrl + C` and `node server.js`

## License
This project is licensed under the MIT License.

