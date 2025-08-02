# Mini LinkedIn-like Community Platform

This project is a simplified LinkedIn-style platform developed as part of the Full Stack Development Internship at CIAAN Cyber Tech Pvt Ltd.

---

## 🚀 Features

### 1. User Authentication
- Register and Login using email and password
- JWT-based login system
- User Profile includes: Name, Email, and Bio

### 2. Public Post Feed
- Create, view, and read **text-only** posts
- Home feed shows post with author name and timestamp

### 3. Profile Page
- View user’s profile and all their posts

### 4. Extra Feature
- File upload API supported using `express-fileupload`
- Protected `/upload` endpoint to upload files

---

## ⚙️ Tech Stack

| Layer      | Technology              |
|------------|--------------------------|
| Frontend   | React + Tailwind CSS     |
| Backend    | Node.js + Express        |
| Database   | MongoDB Atlas            |
| Auth       | JWT (JSON Web Tokens)    |
| Deployment | Vercel (frontend), Render (backend) |

---

## 🛠️ Setup Instructions

### Frontend (Client)

```bash
cd client
npm install
npm run dev
Backend (Server)
bash
Copy
Edit
cd server
npm install
# Setup .env file based on template below
node index.js
🔐 .env Configuration (create in /server)
env
Copy
Edit
MONGODB_URI=your_mongo_db_connection
JWT_SECRET=your_jwt_secret
PORT=5000
🔐 Auth Flow
Token stored in localStorage after login

Protected routes checked with isAuthenticated() function

Logout clears token and reloads app

🌐 Live Demos
🔗 Frontend: https://mini-linkedin-client.vercel.app

🔗 Backend API: https://mini-linkedin-api.onrender.com

👤 Demo Accounts
You can register any test account yourself using the Register page.

📁 File Upload Support
POST /upload with file (e.g. profile photo or resume)

Uploads stored under uploads/ folder and served statically

✅ Project Status
All required features implemented

Basic responsive layout using Tailwind CSS

Fully deployed and working end-to-end
