# 📚 Secure Book API with JWT & React Frontend

A full-stack web application featuring a secure RESTful API built with **Node.js, Express, and MongoDB**, protected by **JSON Web Tokens (JWT)**, and a dynamic **React** frontend with user authentication, local storage token management, and conditional UI rendering.

---

## 🛠️ Tech Stack

### **Backend:**
* **Node.js** & **Express.js** (REST API framework)
* **MongoDB** & **Mongoose** (Database & ODM)
* **JSON Web Token (JWT)** (Authentication)
* **Bcrypt.js** (Password hashing)
* **CORS** & **Dotenv**

### **Frontend:**
* **React** (with Vite)
* **React Router DOM** (Client-side routing)
* **HTML5 / CSS3 / JavaScript (ES6+)**

---

## 📂 Project Directory Structure

```text
book-api-project/
│
├── server/                    # Backend API
│   ├── models/
│   │   └── User.js            # User Mongoose Schema
│   ├── middleware/
│   │   └── auth.js            # JWT Token verification middleware
│   ├── routes/
│   │   ├── auth.js            # /register and /login endpoints
│   │   └── books.js           # Book CRUD routes (Public GET, Protected POST/PUT/DELETE)
│   ├── .env                   # Environment variables
│   ├── .gitignore             # Ignored files (node_modules, .env)
│   ├── package.json
│   └── server.js              # Entry point for Express
│
└── client/                    # Frontend React Application
    ├── src/
    │   ├── components/
    │   │   ├── Navbar.jsx     # Navigation bar with dynamic auth state UI
    │   │   └── Login.jsx      # Login page handling authentication & token storage
    │   ├── App.jsx            # Main app router and Book management dashboard
    │   └── main.jsx
    ├── .gitignore
    ├── index.html
    └── package.json
