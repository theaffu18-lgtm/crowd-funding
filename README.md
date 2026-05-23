📌 Project Overview

The Crowd Funding Application is a full-stack web platform where users can create fundraising campaigns, donate to campaigns, explore active fundraisers, and manage crowdfunding activities securely.

The platform allows:

Users to register/login
Create fundraising campaigns
Upload campaign details and images
Donate to campaigns
Track funding progress
Manage user dashboards
Explore multiple fundraising categories

The application is designed with a modern MERN Stack architecture and focuses on scalability, responsive UI, and secure API communication.

🚀 Features
👤 Authentication & Authorization
User Registration
User Login
JWT Authentication
Protected Routes
Role-Based Access Control
Password Encryption using bcrypt

💰 Campaign Management
Create Campaign
Edit Campaign
Delete Campaign
View Campaign Details
Funding Goal Tracking
Campaign Deadline Management

❤️ Donation System
Donate to Campaigns
Real-Time Funding Updates
Donor Tracking
Funding History

📊 Dashboard
User Dashboard
Campaign Statistics
Donation Tracking
Profile Management

🔍 Search & Filtering
Search Campaigns
Filter by Category
Sort by Funding Status

📱 Responsive UI
Mobile Responsive
Tablet Responsive
Desktop Optimized

🛠️ Tech Stack
Frontend
React.js
React Router DOM
Axios / Fetch API
Tailwind CSS / CSS Modules
Context API / Redux

Backend
Node.js
Express.js
Database
MongoDB
Mongoose ODM
Authentication
JWT (JSON Web Token)
bcryptjs

Deployment
Frontend: Vercel
Backend: Render 

🧠 Application Architecture
Frontend (React)
        ↓
REST API Calls
        ↓
Backend Server (Node + Express)
        ↓
MongoDB Database

🗄️ Database Models

1️⃣ User Model
User Schema
Fields
Field	Type	Description
name	String	User full name
email	String	Unique email
password	String	Encrypted password
role	String	user/admin
profileImage	String	User avatar
createdAt	Date	Account creation date

2️⃣ Campaign Model
Campaign Schema
Fields
Field	Type	Description
title	String	Campaign title
description	String	Campaign details
goalAmount	Number	Target amount
raisedAmount	Number	Collected amount
image	String	Campaign image
category	String	Campaign category
deadline	Date	Funding deadline
creator	ObjectId	Campaign owner
donors	Array	Donation records

3️⃣ Donation Model
Donation Schema
Fields
Field	Type	Description
donor	ObjectId	User reference
campaign	ObjectId	Campaign reference
amount	Number	Donation amount
donatedAt	Date	Donation date

🔗 API Routes
🔐 Authentication Routes
POST /api/auth/register
Description

Register new user

POST /api/auth/login
Description

Login existing user

GET /api/auth/profile
Description

Get logged in user profile

📢 Campaign Routes
GET /api/campaigns
Description

Get all campaigns

GET /api/campaigns/:id
Description

Get single campaign

POST /api/campaigns
Description

Create campaign

PUT /api/campaigns/:id
Description

Update campaign

DELETE /api/campaigns/:id
Description

Delete campaign

❤️ Donation Routes
POST /api/donations
Description

Donate to campaign

GET /api/donations/:campaignId
Description

Get campaign donations

🧩 Middleware
Authentication Middleware
verifyToken()
Purpose
Verifies JWT token
Protects private routes
Error Middleware
errorHandler()
Purpose
Handles server errors globally
Upload Middleware
multer()
Purpose
Handles image uploads

⚙️ Environment Variables

Create .env file in backend folder:

PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:5173

▶️ Installation & Setup
Clone Repository
git clone <your-repository-url>
Install Frontend Dependencies
cd frontend
npm install

Install Backend Dependencies
cd backend
npm install
Start Backend Server
npm run server
Start Frontend
npm run dev

🌐 Deployment
Frontend Deployment

Deployed on:
Vercel

Backend Deployment
Can be deployed using:
Render
Railway
Cyclic

🔒 Security Features
JWT Authentication
Password Hashing
Protected APIs
Secure Environment Variables
CORS Protection
Input Validation

📸 Application Screens
Home Page
Campaign listings
Trending campaigns
Search functionality
Campaign Details
Donation section
Campaign progress
Donor information
Dashboard
User campaigns
Donation history
Profile management

📈 Future Enhancements
Payment Gateway Integration
Real-Time Notifications
Admin Analytics Dashboard
Social Media Sharing
Campaign Comments
AI-Based Campaign Recommendations

👨‍💻 Team Contribution
Role	Responsibility
Frontend Developer	UI/UX Development
Backend Developer	APIs & Database
Database Manager	MongoDB Design
Deployment Manager	Hosting & CI/CD

📚 Learning Outcomes
Through this project we learned:
Full Stack Development
REST API Development
MongoDB Schema Design
Authentication & Authorization
Deployment Process
State Management
Responsive Design

📝 Conclusion
The Crowd Funding Application provides a secure and scalable platform for fundraising activities. It demonstrates complete MERN stack implementation including frontend development, backend APIs, database integration, authentication, and deployment workflows.

The project is built with clean architecture principles and can be extended with advanced production-level features in future updates.
