# README.md

## MERN Project Management System

A full-stack MERN application for managing projects, tasks, analytics, and team collaboration with authentication and responsive UI.

Project Live link: https://mern-frontend-production-bfb4.up.railway.app/

---

# Features

* User Signup & Login Authentication
* JWT Secure Authentication
* Protected Backend APIs
* Create Projects
* Add & Remove Team Members
* Task Assignment System
* Task Status Tracking
* Analytics Dashboard
* Responsive Mobile UI
* Secure Cookie-Based Sessions
* REST API Integration
* MongoDB Database Integration
* Modern Dashboard Interface

---

# Tech Stack

## Frontend

* React.js
* React Router DOM
* CSS
* Lucide React Icons

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcryptjs
* cookie-parser
* cors
* dotenv

---

# Folder Structure

```bash
frontend/
backend/
```

---

# Environment Variables

## Backend `.env`

```env
PORT=5000 (not mandatory)

MONGO_URL=your_mongodb_connection

JWT_SECRET=your_secret_key
```

---

## Frontend `.env`

```env
REACT_APP_API_URL=https://your-backend-url.up.railway.app
```

---

# Backend Setup

```bash
cd backend

npm install

npm start
```

Backend runs on:

```bash
http://localhost:5000
```

---

# Frontend Setup

```bash
cd frontend

npm install

npm start
```

Frontend runs on:

```bash
http://localhost:3000
```

---

# Railway Deployment

## Backend Deployment

1. Push backend code to GitHub

2. Go to Railway

3. Create New Project

4. Deploy from GitHub Repo

5. Add Environment Variables:

```env
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
```

6. Railway generates backend URL:

```bash
https://your-backend.up.railway.app
```

---

## Frontend Deployment

1. Push frontend code to GitHub

2. Create another Railway service

3. Deploy frontend repo

4. Add frontend environment variable:

```env
REACT_APP_API_URL=https://your-backend.up.railway.app
```

5. Redeploy frontend

---

# CORS Configuration

Backend `index.js`

```js
app.use(cors({

    origin:[

        "http://localhost:3000",

        "https://your-frontend.up.railway.app"
    ],

    credentials:true
}));
```

---

# Authentication

* JWT Token Based Authentication
* Protected Backend APIs using Middleware
* Cookies used for session handling

---

# API Routes

## Authentication

```bash
POST /signup-data
POST /login-data
GET  /logout
```

## Dashboard

```bash
GET /dashboard
```

## Projects

```bash
POST /create-project
GET  /projects
PUT  /update-project-status
```

## Members

```bash
POST /add-member
POST /remove-member
```

## Analytics

```bash
GET /get-analytics
```

---

# Deployment Links

## Frontend

```bash
https://your-frontend.up.railway.app
```

## Backend

```bash
https://your-backend.up.railway.app
```

---

# Author

Raziya Chikkale


---

# License

This project is for educational and learning purposes.
