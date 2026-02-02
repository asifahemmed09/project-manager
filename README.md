# 🚀 TeamSync — B2B Project Management Platform

TeamSync is a full-stack, multi-tenant project management platform built for modern teams. It enables secure collaboration through workspace isolation, role-based access control (RBAC), real-time task tracking, and Google OAuth authentication.

---

## 🔗 Live Links

- **Live Demo:** https://team-sync-drab-rho.vercel.app/
- **Backend API:** https://team-sync-api.onrender.com/

---

## ✨ Key Features

### 🔐 Authentication & Authorization
- Google OAuth 2.0 using Passport.js
- Email & password authentication with Bcrypt
- Secure cookie-based session management
- Role-Based Access Control (Owner, Admin, Member)

### 🏢 Workspace Management
- Multi-tenant workspace isolation
- Invite members via secure invite links
- Workspace-level analytics and progress overview

### 📋 Project & Task Management
- Task lifecycle: Backlog → To-Do → In Progress → Done
- Advanced filtering by status, priority, and assignee
- Project-level task isolation with custom branding & emojis
- URL-based filter state management using `nuqs`

---

## 🛠️ Tech Stack

### Frontend
- React 18 (Vite)
- TypeScript
- TanStack Query (React Query)
- Tailwind CSS + Shadcn UI
- React Router DOM v6
- React Hook Form + Zod

### Backend
- Node.js (Express)
- MongoDB + Mongoose
- Passport.js (Local & Google strategies)
- Zod validation

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/asifahemmed09/project-manager.git
cd project-manager
```

### 2️⃣ Install Dependencies
```bash
# Frontend
cd client
npm install

# Backend
cd ../server
npm install
```

### 3️⃣ Environment Variables

Create a `.env` file inside the `server` directory:

```env
NODE_ENV=development
PORT=5000

MONGO_URI=your_mongodb_uri
SESSION_SECRET=your_session_secret

GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_CALLBACK_URL=http://localhost:5000/api/auth/google/callback

FRONTEND_ORIGIN=http://localhost:5173
FRONTEND_GOOGLE_CALLBACK_URL=http://localhost:5173/google/oauth/callback
```

### ▶️ Running the Application

**Start Backend**
```bash
cd server
npm run dev
```

**Start Frontend**
```bash
cd client
npm run dev
```

- **Frontend:** http://localhost:5173  
- **Backend API:** http://localhost:5000

---


## 🛡️ License

MIT License

Copyright (c) 2026 Asif Ahemmed

---

## 📬 Contact

**Asif Ahemmed**

- Email: asifahemmed.dev@gmail.com
- Project Repository: https://github.com/asifahemmed09/project-manager

---

⭐ **If you find this project helpful, please consider giving it a star!**
