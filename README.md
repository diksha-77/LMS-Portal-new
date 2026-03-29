Learning Management System (LMS)
 Overview

The Learning Management System (LMS) is a web application that allows users to manage and access online courses. It provides features for students to enroll in courses and for admins to manage course content.

Features
User Registration & Login
Role-based access (Admin / Student)
Course creation and management
Student enrollment in courses
Access to study materials
Dashboard for users

Tech Stack
Frontend: React.js, HTML, CSS, JavaScript
Backend: Node.js, Express.js
Database: MongoDB Atlas


Project Structure
LMS-Portal/
│
├── client/        # Frontend (React)
├── server/        # Backend (Node + Express)
├── models/        # Database schemas
├── routes/        # API routes
├── controllers/   # Logic
├── .env           # Environment variables
└── README.md


Setup Instructions
1. Clone the repository
git clone https://github.com/your-username/LMS-Portal.git
cd LMS-Portal
2. Install dependencies

Backend

cd server
npm install

Frontend

cd client
npm install
3. Configure Environment Variables

Create a .env file inside the server folder:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
4. Run the project

Start Backend
npm start

Start Frontend
npm start

🔌 API Endpoints
POST /api/auth/register → Register user
POST /api/auth/login → Login user
GET /api/courses → Get all courses
POST /api/courses → Create course
