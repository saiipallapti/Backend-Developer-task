Backend Developer (Intern) – Project Assignment

A full-stack application implementing secure authentication, role-based access control, and CRUD operations using React, Node.js, Express, and MongoDB Atlas.

This project demonstrates the design of a secure, scalable REST API with a simple frontend UI for testing and interacting with backend services.

🚀 Tech Stack
Backend

Node.js

Express.js

MongoDB Atlas

JWT Authentication

bcrypt for password hashing

Frontend

React.js

Vite

Axios

Tools

Thunder Client / Postman

Git & GitHub

Nodemon

📌 Assignment Overview

The goal of this assignment is to:

Build a secure REST API

Implement JWT authentication

Implement role-based access control

Build CRUD APIs

Create a basic frontend UI to test APIs

Follow security and scalability best practices

✅ Core Features
Backend (Primary Focus)

User registration & login

Password hashing using bcrypt

JWT authentication with expiration

Role-based access (User / Admin)

CRUD APIs for Tasks

API versioning

Input validation & error handling

MongoDB Atlas database integration

🎨 Frontend (Supportive)

Simple React UI that allows users to:

Register account

Login and receive JWT token

Access protected dashboard

Perform CRUD operations on tasks

Display API success/error messages

🔐 Security & Scalability

Security practices implemented:

Password hashing using bcrypt

JWT authentication for protected routes

Role-based access control

Input validation

Structured project architecture

Scalability considerations:

Modular backend architecture

Easy addition of new modules

Ready for microservices architecture

Can integrate Redis caching

Docker-ready deployment

📁 Project Structure
backend-intern-task
│
├── backend
│   ├── controllers
│   │   ├── authController.js
│   │   └── taskController.js
│   │
│   ├── middleware
│   │   └── auth.js
│   │
│   ├── models
│   │   ├── User.js
│   │   └── Task.js
│   │
│   ├── routes
│   │   ├── auth.js
│   │   └── tasks.js
│   │
│   ├── server.js
│   └── package.json
│
├── frontend
│   ├── src
│   ├── package.json
│   └── vite.config.js
│
├── Postman_Collection.json
└── README.md
⚙️ Running the Project Locally
1️⃣ Clone Repository
git clone https://github.com/yourusername/backend-intern-task.git
cd backend-intern-task
Backend Setup
cd backend
npm install
npx nodemon server.js

Server runs on:

http://localhost:5000
Frontend Setup
cd frontend
npm install
npm run dev

Frontend runs on:

http://localhost:5179
🔑 Authentication Flow

1️⃣ User registers with email & password
2️⃣ Password hashed using bcrypt
3️⃣ User logs in and receives JWT token
4️⃣ Token stored in localStorage
5️⃣ Token sent in Authorization header for protected routes

Example:

Authorization: Bearer <token>
💻 API Routes
Authentication
Method	Route	Description
POST	/api/v1/auth/register	Register new user
POST	/api/v1/auth/login	Login user
Task Routes (Protected)
Method	Route	Description
GET	/api/v1/tasks	Get all tasks
POST	/api/v1/tasks	Create task
PUT	/api/v1/tasks/:id	Update task
DELETE	/api/v1/tasks/:id	Delete task
🧪 API Testing

All APIs tested using:

Thunder Client

Postman

Collection file included:

Postman_Collection.json
⚡ Scalability Notes

This system can scale by:

Splitting services into microservices

Adding Redis caching

Implementing load balancing

Using Docker containers

👨‍💻 Author

Saii Pallapati

📧 Email
saiiipallapati@gmail.com

📱 Phone
+91 7780238400
