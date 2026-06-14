# 🌿 GreenCRM - Full Stack CRM Application

A complete CRM system built with Node.js/Express backend and React frontend.

## Tech Stack

**Backend:** Node.js, Express, MongoDB, Mongoose, JWT Auth  
**Frontend:** React, Vite, Tailwind CSS, Recharts, React Router

---

## Quick Start

### 1. Install Backend Dependencies
```bash
cd backend
npm install
```

### 2. Configure Backend
Edit `backend/.env`:
```
MONGODB_URI=mongodb://localhost:27017/greencrm
PORT=5005
JWT_SECRET=your_secret_key_here
JWT_EXPIRE=7d
```

### 3. Start Backend
```bash
cd backend
npm run dev
```

### 4. Install Frontend Dependencies
```bash
cd frontend
npm install
```

### 5. Start Frontend
```bash
cd frontend
npm run dev
```

Frontend runs at **http://localhost:3000**  
Backend API runs at **http://localhost:5005**

---

## Features

- **Authentication** — Register/Login with JWT, role-based access (Admin, Manager, Sales Executive)
- **Dashboard** — Stats overview, deal/lead charts, recent activity feed
- **Customers** — Full CRUD, search, status & source filtering
- **Leads** — Pipeline management with status, priority, estimated value
- **Deals** — Deal tracking with stages, probability, customer linking
- **Tasks** — Task management with due dates, priorities, one-click complete
- **Activities** — Activity log (Email, Call, Meeting, Note, Task, Deal Update)

---

## Project Structure

```
greencrm/
├── backend/
│   ├── config/database.js
│   ├── middleware/auth.js
│   ├── models/          # User, Customer, Lead, Deal, Task, Activity
│   ├── routes/          # auth, customers, leads, deals, tasks, activities, dashboard
│   ├── server.js
│   ├── .env
│   └── package.json
└── frontend/
    ├── src/
    │   ├── components/Layout.jsx
    │   ├── context/AuthContext.jsx
    │   ├── pages/       # Login, Register, Dashboard, Customers, Leads, Deals, Tasks, Activities
    │   ├── utils/api.js
    │   ├── styles/index.css
    │   └── App.jsx
    ├── .env
    ├── vite.config.js
    ├── tailwind.config.js
    └── package.json
```
