# 🚀 Crowd Funding Frontend

## 📌 Overview

The frontend is built using **React + Vite** and provides the user interface for the crowdfunding platform.

### Features

- User Authentication
- Campaign Creation
- Donation System
- Dashboard Management
- Analytics
- Responsive Design

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|----------|
| React | Frontend Library |
| Vite | Build Tool |
| Tailwind CSS | Styling |
| Axios | API Requests |
| Zustand | State Management |
| React Router DOM | Routing |
| Chart.js | Analytics |

---

# 📂 Folder Structure

```bash
client/
│
├── public/
│
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── routes/
│   ├── services/
│   ├── store/
│   ├── App.jsx
│   └── main.jsx
│
├── package.json
└── vite.config.js
```

---

# ⚡ Important Files

## main.jsx

Entry point of the React application.

### Responsibilities

- Renders React app
- Loads global styles
- Connects App component to DOM

---

## App.jsx

Main application component.

### Responsibilities

- Defines routes
- Handles navigation
- Loads layouts and pages

---

# 🔐 Authentication Flow

```text
User Login
    ↓
Frontend Validation
    ↓
API Request
    ↓
Backend Verification
    ↓
JWT Token Generated
    ↓
Access Granted
```

---

# 🎯 Campaign Flow

```text
Create Campaign
      ↓
Upload Image
      ↓
Store Campaign
      ↓
Display Publicly
```

---

# 💳 Donation Flow

```text
User Donates
      ↓
Razorpay Order Created
      ↓
Payment Gateway Opens
      ↓
Payment Success
      ↓
Donation Stored
```

---

# 🌐 API Communication

Axios is used for backend communication.

```js
axios.post("/api/auth/login", data)
```

---

# ⚙️ Environment Variables

Create `.env` inside client folder:

```env
VITE_API_URL=http://localhost:5000
```

---

# ▶️ Running Frontend

## Install Dependencies

```bash
npm install
```

## Start Development Server

```bash
npm run dev
```

---

# ✨ Frontend Features

## 👤 User Features

- Register/Login
- Create Campaign
- Donate
- Manage Dashboard

## 🛡️ Admin Features

- Manage Users
- Campaign Moderation
- Analytics Dashboard
