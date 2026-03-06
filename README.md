# Backend Developer (Intern) – Project Assignment

A full-stack project implementing secure user authentication, role-based access, and CRUD operations using **React, Node.js, Express, and MongoDB Atlas**.

This project demonstrates a scalable backend system with a simple frontend UI for testing APIs.

---

# 🚀 Project Structure

```
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
```

---

# ⚙️ Running the Project Locally

## 1️⃣ Clone Repository

```
git clone https://github.com/yourusername/backend-intern-task.git
cd backend-intern-task
```

---

# Backend Setup

```
cd backend
npm install
npx nodemon server.js
```

Server runs on:

```
http://localhost:5000
```

---

# Frontend Setup

```
cd frontend
npm install
npm run dev
```

Frontend runs on:

```
http://localhost:5179
```

---

# 🔑 Authentication Flow

1️⃣ User registers with email and password  
2️⃣ Password hashed using **bcrypt**  
3️⃣ User logs in and receives **JWT token**  
4️⃣ Token stored in **localStorage**  
5️⃣ Token sent in **Authorization header** for protected routes  

Example:

```
Authorization: Bearer <token>
```

---

# 💻 API Routes

## Authentication

| Method | Route | Description |
|------|------|------|
| POST | /api/v1/auth/register | Register new user |
| POST | /api/v1/auth/login | Login user |

---

# Task Routes (Protected)

| Method | Route | Description |
|------|------|------|
| GET | /api/v1/tasks | Get all tasks |
| POST | /api/v1/tasks | Create task |
| PUT | /api/v1/tasks/:id | Update task |
| DELETE | /api/v1/tasks/:id | Delete task |

---

# 🧪 API Testing

All APIs tested using:

- Thunder Client
- Postman

Collection included:

```
Postman_Collection.json
```

---

# ⚡ Scalability Notes

This system can scale using:

- Microservices architecture
- Redis caching
- Load balancing
- Docker containers

---

# 👨‍💻 Author

**Saii Pallapati**

📧 Email:  
saiiipallapati@gmail.com

📱 Phone:  
+91 7780238400
