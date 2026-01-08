# MERN Authentication System with Email Verification and Password Reset

A complete authentication system built with the MERN stack (MongoDB, Express, React, Node.js) featuring email verification, secure password reset with OTP, and JWT-based authentication.

## Overview

Registration and Password Reset system using MERN Stack | JWT Authentication And Email Verification OTP In React Project.

In this project we build a complete Authentication system that includes:
- **Email Verification** with OTP authentication
- **Password Reset Feature** using a secure 6-digit OTP sent directly to user's email
- **JWT Authentication** for secure session management
- **Modern Frontend** built with React and Tailwind CSS

## Project Architecture

### Backend
We build our Backend server to create APIs to manage Authentication requests using:
- **MongoDB** - NoSQL Database for user data storage
- **Express.js** - REST API framework
- **Node.js** - Server runtime
- **JWT (JsonWebToken)** - Secure authentication tokens
- **Nodemailer** - Email service for OTP delivery

### Frontend
We build our client app with:
- **React** - UI framework with hooks and components
- **Tailwind CSS** - Responsive styling
- **Vite** - Fast development build tool

## Features

✅ User Registration with Email Verification
✅ Secure Password Reset with 6-digit OTP
✅ JWT Token-based Authentication
✅ Email Verification OTP
✅ Login/Register Forms with OTP Input Field
✅ Password Reset Forms
✅ Protected Routes and API Endpoints
✅ Responsive Design
✅ React Hooks and Components
✅ MongoDB Integration

## Run Locally

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Setup Backend Server

1. Navigate to server directory
```bash
cd server
```

2. Install dependencies
```bash
npm install
```

3. Create `.env` file in server directory with:
```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
```

4. Start the server
```bash
npm start
```

Server will run on `http://localhost:5000` (or your configured PORT)

### Setup Frontend Client

1. Navigate to client directory
```bash
cd client
```

2. Install dependencies
```bash
npm install
```

3. Create `.env` file in client directory with:
```
VITE_API_URL=http://localhost:5000
```

4. Start the development server
```bash
npm run dev
```

Client will run on `http://localhost:5173` (Vite default)

## API Endpoints

### Authentication Routes
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/send-reset-otp` - Send password reset OTP
- `POST /api/auth/reset-password` - Reset password with OTP
- `POST /api/auth/verify-email` - Verify email with OTP

### User Routes
- `GET /api/user/profile` - Get user profile (Protected)
- `PUT /api/user/profile` - Update user profile (Protected)

## Key Technologies

- **Authentication:** JWT (JSON Web Tokens)
- **Database:** MongoDB with Mongoose ODM
- **Email Service:** Nodemailer
- **Frontend Framework:** React with Hooks
- **Styling:** Tailwind CSS
- **Build Tool:** Vite
- **API:** Express.js REST API

## Project Structure

```
MERN-AUTH/
├── client/                 # React Frontend
│   ├── src/
│   │   ├── components/    # React Components
│   │   ├── pages/         # Page Components
│   │   ├── context/       # App Context
│   │   └── assets/        # Static Assets
│   └── package.json
└── server/                 # Node.js Backend
    ├── config/            # Configuration Files
    ├── controllers/       # Route Controllers
    ├── models/           # Database Models
    ├── routes/           # API Routes
    ├── middleware/       # Custom Middleware
    └── package.json
```

## Learning Outcomes

By following this project, you will learn:
- How to build a complete authentication system from scratch
- JWT token implementation and best practices
- Email verification and OTP handling
- MERN stack development
- RESTful API design
- React hooks and state management
- Form handling and validation
- Database design with MongoDB

## Notes

- Passwords are hashed using bcrypt for security
- OTP codes are temporarily stored and expire after a set time
- JWT tokens include expiration for enhanced security
- Email templates are customizable for different languages

## License

This is a learning project created for educational purposes.

## Credits

Built as a learning exercise following MERN stack tutorials and best practices.
