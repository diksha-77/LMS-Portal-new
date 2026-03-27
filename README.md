📚 Learning Management System (LMS)
🚀 Project Description

The Learning Management System (LMS) is a full-stack web application designed to streamline the management of online learning. It enables instructors to create and manage courses while allowing students to enroll, access materials, and track their progress in a centralized platform.

🎯 Key Highlights
Full-stack MERN application with RESTful API architecture
Secure authentication and authorization using JWT
Scalable database design using MongoDB Atlas
Modular backend with MVC structure
Responsive and user-friendly UI


✨ Features
👤 Authentication & Authorization
User registration and login
Role-based access (Admin / Student)
JWT-based authentication


📖 Course Management
Create, update, and delete courses (Admin)
View all available courses (Students)


🎓 Enrollment System
Students can enroll in courses
Track enrolled courses

📊 Dashboard
Personalized user dashboard
Course tracking and activity overview


🛠️ Tech Stack
Frontend
React.js
HTML5, CSS3
JavaScript (ES6+)


Backend
Node.js
Express.js

Database
MongoDB Atlas

Tools & Libraries
Mongoose (ODM)
JSON Web Token (JWT)
dotenv
Postman (API Testing)


🏗️ Architecture

The project follows a MVC (Model-View-Controller) architecture:

server/
│
├── models/        # MongoDB schemas
├── controllers/   # Application logic
├── routes/        # API routes
├── middleware/    # Auth & error handling
├── config/        # DB configuration
└── server.js      # Entry point
📁 Project Structure

LMS-Portal/
│
├── client/            # React frontend
│   ├── src/
│   └── public/
│
├── server/            # Backend (Node + Express)
│
├── .env               # Environment variables
├── package.json
└── README.md

⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/your-username/LMS-Portal.git
cd LMS-Portal
2️⃣ Backend Setup
cd server
npm install

Create .env file:

PORT=5000
MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=your_secret_key

Run backend:

npm run dev
3️⃣ Frontend Setup
cd client
npm install
npm start

🔌 API Overview
Auth Routes
POST /api/auth/register → Register user
POST /api/auth/login → Login user

Course Routes
GET /api/courses → Fetch all courses
POST /api/courses → Create course (Admin)
PUT /api/courses/:id → Update course
DELETE /api/courses/:id → Delete course

Enrollment Routes
POST /api/enroll/:courseId → Enroll in course
🔐 Security Features
Password hashing using bcrypt
JWT-based authentication
Protected routes using middleware
