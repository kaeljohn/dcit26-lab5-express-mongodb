# Student Records REST API

A backend service built with Node.js, Express, MongoDB, and Mongoose for managing student records.

## Setup Instructions

1. Clone repository:
   git clone <your-repo-url>
   cd dcit26-lab5-express-mongodb

2. Install dependencies:
   npm install

3. Environment Setup:
   Copy `.env.example` to `.env`:
   cp .env.example .env
   Ensure MongoDB is running locally (`mongodb://127.0.0.1:27017/lab5_students`).

4. Run the server:
   npm run dev    # Development mode (nodemon)
   npm start      # Production mode

## API Routes

| Method | Endpoint            | Description                          | Success Code |
| ------ | ------------------- | ------------------------------------ | ------------ |
| GET    | `/api/health`       | Check API and server status          | 200          |
| GET    | `/api/students`     | Fetch all student records            | 200          |
| GET    | `/api/students/:id` | Fetch a single student record by ID  | 200          |
| POST   | `/api/students`     | Create a new student record          | 201          |
| PUT    | `/api/students/:id` | Update an existing student record    | 200          |
| DELETE | `/api/students/:id` | Delete a student record by ID        | 200          |