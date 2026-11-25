LinkedIn Clone – MERN Stack Project

A full-stack professional networking platform inspired by LinkedIn, built using the **MERN Stack (MongoDB, Express.js, React.js, and Node.js)**. This project allows users to create professional profiles, connect with other professionals, share posts, interact with content, and build their professional network.

The primary objective of this project is to develop a real-world social networking application with secure authentication, dynamic user profiles, image uploads, and interactive features.

---

## 🚀 Features

### 1. Authentication & Authorization
- User Registration and Login.
- Secure password hashing using Bcrypt.
- JWT-based authentication.
- HTTP-only cookies for secure token storage.
- Protected routes using authentication middleware.
- User Logout functionality.

### 2. User Profile Management
- Create and update user profiles.
- Upload and update profile pictures.
- Upload and update cover images.
- Add professional headlines.
- Manage personal information and location.
- Add and update skills.
- Manage educational qualifications.
- Add and manage professional experience.

### 3. Social Networking
- Connect with other professionals.
- View other users' profiles.
- Build a professional network.
- Discover other users.

### 4. Post Management
- Create and publish posts.
- Upload images with posts.
- View posts from other users.
- Like and interact with posts.
- Delete or manage posts.

### 5. Media Management
- Image uploads using Multer.
- Cloudinary integration for cloud-based image storage.
- Profile and cover image management.

---

## 🛠️ Tech Stack

### Frontend
- React.js
- JavaScript (ES6+)
- Tailwind CSS
- Axios
- React Router DOM
- React Icons
- React Context API

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- Bcrypt.js
- Cookie Parser
- Multer
- Cloudinary
- dotenv
- CORS

### Development Tools
- Visual Studio Code
- Git & GitHub
- Postman
- MongoDB Atlas
- Cloudinary

---

## 📁 Project Structure

text
LinkedIn-Clone/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── uploads/
│   ├── .env
│   ├── .gitignore
│   ├── index.js
│   └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── .env
│   ├── .gitignore
│   └── package.json
│
├── .gitignore
└── README.md


*Note: The folder structure may vary depending on the implementation.*

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally.

### 1. Clone the Repository

bash
git clone YOUR_GITHUB_REPOSITORY_URL

bash
cd LinkedIn-Clone


### 2. Backend Setup

Navigate to the backend directory:

bash
cd backend


Install dependencies:

bash
npm install

Create a `.env` file in the backend directory:

env
PORT=8000
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret


Start the backend server:

bash
npm run dev

The backend server will run on:

http://localhost:8000

 
3. Frontend Setup

Open another terminal and navigate to the frontend directory:

bash
cd frontend

Install dependencies:

bash
npm install

Create a `.env` file in the frontend directory:

env
VITE_API_URL=http://localhost:8000


Start the frontend development server:

bash
npm run dev


The frontend application will run on:

http://localhost:5173

---

## 🔐 Environment Variables

For security reasons, never upload your `.env` files or expose your secret credentials on GitHub.

Make sure the following files are included in your `.gitignore`:

gitignore
node_modules/
.env
.env.*
!.env.example
dist/

Create `.env.example` files containing placeholder values to help other developers configure the project.


## 🔄 Application Workflow

1. A new user registers using their personal details.
2. The backend validates the information and securely hashes the password.
3. User information is stored in MongoDB.
4. After successful login, a JWT token is generated.
5. The authentication token is stored in
