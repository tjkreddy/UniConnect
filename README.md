# UniConnect
# 🚀 MU-UniConnect

A comprehensive platform designed for Mahindra University's ecosystem, connecting students, faculty, and club administrators in one unified digital space.

![UniConnect Banner](client/public/img/UNICONNECT.png)

## 📌 Overview

MU-UniConnect is a full-stack web application built to streamline university communications, event management, faculty appointments, and campus activities. It serves as a central hub for the entire university community with role-specific features and dashboards.

## ✨ Key Features

- **User Authentication & Authorization**
  - Role-based access control (students, faculty, club heads, administrators)
  - Secure login and registration with email verification
  - Password reset functionality

- **Faculty Management**
  - Faculty profiles and availability scheduling
  - Appointment booking system for students
  - Office hours management

- **Campus Life**
  - Club management and event creation
  - Campus highlights and announcements
  - Interactive campus map with key locations

- **Academic Tools**
  - Calendar integration with university events
  - Rich text editing for presentations and announcements
  - Feedback submission system

- **Admin Dashboard**
  - User management interface
  - Content moderation tools
  - System-wide announcements

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI library
- **React Router** - Navigation and routing
- **TailwindCSS** - Styling and UI components
- **Framer Motion** - Animations
- **React Hook Form** - Form validation
- **Axios** - API requests
- **React Quill** & **TipTap** - Rich text editing
- **React Big Calendar** - Event scheduling

### Backend
- **Node.js** & **Express** - Server framework
- **MongoDB** & **Mongoose** - Database and ODM
- **JWT** - Authentication
- **Multer** - File uploads
- **Nodemailer** - Email functionality

## 🏗️ Project Structure

This repository contains both frontend and backend code:
- **Frontend (React)**: Located in the `client` directory
- **Backend (Node.js/Express)**: Located in the `server` directory

```
uniconnect/
├── client/                # Frontend React application
│   ├── public/            # Static assets
│   └── src/               # React source code
│       ├── components/    # Reusable UI components
│       ├── contexts/      # React context providers
│       ├── pages/         # Application pages
│       ├── services/      # API service integrations
│       └── utils/         # Utility functions
└── server/                # Backend Node.js application
    ├── config/            # Server configuration
    ├── controllers/       # API route controllers
    ├── middleware/        # Express middlewares
    ├── models/            # Mongoose data models
    ├── routes/            # API route definitions
    └── utils/             # Helper utilities
```

## 🚀 Setup Instructions

### Prerequisites
- Node.js (v14+ recommended)
- MongoDB
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/mu-uniconnect.git
   cd mu-uniconnect
   ```

2. **Install dependencies (both client & server)**
   ```bash
   npm install
   ```
   This will install dependencies for both client and server

### Backend Setup
1. Navigate to the server directory:
   ```bash
   cd server
   ```
   
2. Create a `.env` file in the server directory with the following variables:
   ```env
   PORT=9000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   JWT_LIFETIME=1d
   EMAIL_HOST=smtp.example.com
   EMAIL_PORT=587
   EMAIL_USERNAME=your-email@example.com
   EMAIL_PASSWORD=your-email-password
   EMAIL_FROM=no-reply@mu-uniconnect.com
   ```

3. Start the server:
   ```bash
   npm start
   ```
   or for development:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the client directory:
   ```bash
   cd client
   ```
   
2. Create a `.env` file in the client directory:
   ```env
   REACT_APP_API_URL=http://localhost:9000/api
   ```

3. Start the frontend application:
   ```bash
   npm start
   ```

### Running the Full Application
From the root directory, you can start both frontend and backend concurrently:
```bash
npm run dev
```

## 📚 API Documentation

The server runs on port 9000 by default and provides RESTful API endpoints at `/api/`.

Key API endpoints include:

- **Authentication**: `/api/auth/` - User registration, login, password resets
- **Faculty**: `/api/faculty/` - Faculty profiles and availability
- **Appointments**: `/api/appointments/` - Student-faculty meeting scheduling 
- **Clubs**: `/api/clubs/` - Club information and management
- **Events**: `/api/events/` - University events and activities
- **Campus Highlights**: `/api/campus-highlights/` - Featured campus content

## 🔒 Environment Variables

This project uses environment variables for configuration. Create the following `.env` files:

**Server (.env in server directory)**
```
PORT=9000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_LIFETIME=1d
EMAIL_HOST=smtp.example.com
EMAIL_PORT=587
EMAIL_USERNAME=your-email@example.com
EMAIL_PASSWORD=your-email-password
EMAIL_FROM=no-reply@mu-uniconnect.com
```

**Client (.env in client directory)**
```
REACT_APP_API_URL=http://localhost:9000/api
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 👥 Team

- Lead Developer - [Your Name](https://github.com/yourusername)
- Contributors - [List team members here]

<p align="center">
  Built with ❤️ for Mahindra University
</p>
