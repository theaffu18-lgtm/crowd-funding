# 🛡️ Crowd Funding Backend

## 📌 Overview

The backend is built using **Node.js + Express.js**.

It handles:

- Authentication
- Campaign APIs
- Razorpay Payments
- MongoDB Database
- File Uploads
- Admin Controls

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|----------|
| Node.js | Runtime |
| Express.js | Backend Framework |
| MongoDB | Database |
| Mongoose | ODM |
| JWT | Authentication |
| bcrypt | Password Hashing |
| Razorpay | Payments |
| Cloudinary | Image Storage |

---

# 📂 Folder Structure

```bash
server/
│
├── Apis/
├── Controllers/
├── Models/
├── Middlewares/
├── Database/
├── config/
├── server.js
└── package.json
```

---

# 🏗️ Backend Architecture

```text
Routes
   ↓
Controllers
   ↓
Models
   ↓
MongoDB
```

---

# 🔐 Authentication Flow

## Registration

```text
User Registers
      ↓
Password Hashed
      ↓
User Stored in MongoDB
```

## Login

```text
Credentials Verified
       ↓
JWT Token Generated
       ↓
Token Returned to Frontend
```

---

# 💳 Razorpay Payment Flow

```text
Frontend Requests Order
        ↓
Backend Creates Razorpay Order
        ↓
Payment Popup Opens
        ↓
Payment Successful
        ↓
Donation Saved
```

---

# ☁️ Cloudinary Integration

Cloudinary is used for storing campaign images.

### Benefits

- Cloud image hosting
- Faster image delivery
- Reduced server storage

---

# 🌐 API Examples

## Authentication APIs

```bash
POST /api/auth/register
POST /api/auth/login
```

## Campaign APIs

```bash
GET /api/campaigns
POST /api/campaign/create
PUT /api/campaign/update
DELETE /api/campaign/delete
```

## Payment APIs

```bash
POST /api/payment/create-order
POST /api/payment/verify
```

---

# ⚙️ Environment Variables

Create `.env` inside server folder:

```env
PORT=5000

MONGO_URI=your_mongodb_url

JWT_SECRET=your_secret

RAZORPAY_KEY_ID=your_key

RAZORPAY_SECRET=your_secret

CLOUDINARY_CLOUD_NAME=your_name
CLOUDINARY_API_KEY=your_key
CLOUDINARY_API_SECRET=your_secret
```

---

# ▶️ Running Backend

## Install Dependencies

```bash
npm install
```

## Start Backend

```bash
nodemon server.js
```

or

```bash
npm start
```

---

# 🔒 Security Features

- Password Hashing
- JWT Verification
- Protected Routes
- Middleware Validation

---

# 📚 Learning Concepts

This project helps in learning:

- MERN Stack Development
- REST APIs
- JWT Authentication
- MongoDB Integration
- Razorpay Integration
- State Management
- Protected Routes
- Full Stack Architecture
