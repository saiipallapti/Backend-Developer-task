
# Backend Developer (Intern) – Project Assignment

A full-stack project implementing **secure user authentication, role-based access, and CRUD operations** using React, Node.js, Express, and MongoDB Atlas. This project demonstrates a scalable backend system with a simple frontend UI for testing the APIs.  

---

## 🚀 Assignment Overview

- Build a **Scalable REST API** with authentication and role-based access  
- Implement **CRUD APIs** for a secondary entity (Tasks)  
- Create a **basic frontend UI** to demonstrate API functionality  
- Ensure **security and scalability** best practices  

---

## ✅ Core Features

### **Backend (Primary Focus)**

- User registration & login with **hashed passwords**  
- **JWT authentication** with token expiration  
- **Role-based access** (user vs admin)  
- CRUD APIs for **Tasks** (secondary entity)  
- API versioning, error handling, and validation  
- Database schema using **MongoDB Atlas**  

### **Frontend (Supportive)**

- React.js frontend with simple UI  
- Register & login users  
- Access **protected dashboard** (JWT required)  
- Perform CRUD actions on Tasks  
- Display backend **error/success messages**  

### **Security & Scalability**

- Secure JWT token handling  
- Input sanitization & validation  
- Scalable project structure for new modules  
- Optional: caching (Redis), logging, Docker deployment  

---

## 📁 Project Structure

```text
backend-intern-task/
├── backend/
│   ├── controllers/     # authController.js, taskController.js
│   ├── middleware/      # auth.js (JWT & role checking)
│   ├── models/          # User.js, Task.js
│   ├── routes/          # auth.js, tasks.js
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── src/
│   ├── package.json
│   └── vite.config.js
├── README.md
└── Postman_Collection.json
````

---

## ⚙️ How to Run Locally

### **Backend**

```bash
cd backend
npm install
npx nodemon server.js
```

* Server runs on: `http://localhost:5000`

### **Frontend**

```bash
cd frontend
npm install
npm run dev
```

* Frontend runs on: `http://localhost:5179`

---

## 🔐 Authentication & Role-Based Access Flow

1. User registers with email and password
2. Password is hashed using **bcrypt**
3. User logs in, backend generates **JWT token**
4. JWT stored in **localStorage** on frontend
5. Dashboard and CRUD routes accessible only with valid JWT
6. Role-based access ensures certain routes/actions are **admin-only**
7. Logout clears token

---

## 💻 API Routes

### **Auth Routes**

| Method | Route                 | Description       |
| ------ | --------------------- | ----------------- |
| POST   | /api/v1/auth/register | Register new user |
| POST   | /api/v1/auth/login    | Login and get JWT |

### **Task Routes (Protected)**

| Method | Route             | Description                      |
| ------ | ----------------- | -------------------------------- |
| GET    | /api/v1/tasks     | Get all tasks for logged-in user |
| POST   | /api/v1/tasks     | Create a new task                |
| PUT    | /api/v1/tasks/:id | Update a task by ID              |
| DELETE | /api/v1/tasks/:id | Delete a task by ID              |

> All Task routes require **JWT token in the Authorization header**:
> `Authorization: Bearer <token>`

---

## 📝 Frontend Integration

* Login/Register pages call backend APIs using **Axios**
* JWT token sent in **Authorization header** for protected routes
* CRUD actions for Tasks are reflected in the UI
* Backend **error/success messages** displayed to the user

---

## 🔒 Security Practices

* Passwords hashed using **bcrypt**
* JWT authentication for all protected routes
* Role-based access (`user` vs `admin`)
* Input validation and proper error handling

---

## ⚡ Scalability & Deployment Notes

* Modular project structure allows easy addition of new modules
* Can be scaled with **microservices architecture**
* Optional **Redis caching** for improved performance
* Ready for **Docker deployment** and load balancing

---

## 🧰 API Documentation

* Postman / Thunder Client collection included (`Postman_Collection.json`)
* All APIs tested and functional

---

## 👤 Author

**Saii Pallapati**

* Email: [saiiipallapati@gmail.com](mailto:saiiipallapati@gmail.com)
* Phone: +91 7780238400

---


```

---

