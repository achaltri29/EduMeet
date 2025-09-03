# EduMeet – A WebRTC-Based Video Calling System for Virtual Classrooms

EduMeet is a browser-based, real-time video conferencing web app designed for students and educators. It aims to replicate the core features of platforms like Zoom or Google Meet while remaining lightweight, privacy-conscious, and focused on virtual classroom experiences.

## Features

* **Secure Authentication** – Login and register using JWT tokens and Bcrypt-hashed credentials
* **Join via Meeting Code** – Create or join meetings through unique room codes
* **Real-Time Video & Audio Calling** – Peer-to-peer streaming using WebRTC
* **Live Chat** – Real-time text chat during video sessions via Socket.IO
* **Screen Sharing** – Share your entire screen or a specific tab
* **Meeting History** – Track past sessions with time and date
* **STUN Server Integration** – For NAT traversal in P2P connections
* **Simple UI/UX** – Built with ReactJS and Material UI for responsive, modern design

## 🛠Tech Stack

### Frontend
* **ReactJS**
* **Material UI**
* **WebRTC**
* **Axios**

### Backend
* **Node.js**
* **Express.js**
* **Socket.IO**
* **MongoDB Atlas**
* **Bcrypt** for password hashing
* **JWT** for authentication


## Deployment

### Backend Deployment on Render
The backend is available at: https://edumeetbackend.onrender.com

**Test the Backend Deployment**
* Health check: https://edumeetbackend.onrender.com/api/health
* Root endpoint: https://edumeetbackend.onrender.com/
* User endpoints: https://edumeetbackend.onrender.com/api/users

### Frontend Deployment on Render
The frontend is available at: https://edumeetfrontend.onrender.com

## 📁 Project Structure
```
EduMeet/
├── Backend/
│   ├── src/
│   │   ├── app.js              # Express server with Socket.IO integration
│   │   ├── controllers/
│   │   │   ├── socketManager.js # Socket.IO connection management
│   │   │   └── user.controller.js # User authentication logic
│   │   ├── models/
│   │   │   ├── meeting.model.js # Meeting data schema
│   │   │   └── user.model.js    # User data schema
│   │   └── routes/
│   │       └── users.routes.js  # User authentication routes
│   ├── package.json            # Backend dependencies
│   └── package-lock.json       # Dependency lock file
├── frontend/
│   ├── public/
│   │   ├── index.html          # Main HTML file
│   │   ├── manifest.json       # PWA manifest
│   │   └── icons/              # App icons
│   ├── src/
│   │   ├── App.js              # Main React component
│   │   ├── App.css             # Global styles
│   │   ├── environment.js      # Environment configuration
│   │   ├── contexts/
│   │   │   └── AuthContext.jsx # Authentication context
│   │   ├── pages/
│   │   │   ├── authentication.jsx # Login/Register page
│   │   │   ├── home.jsx        # Dashboard page
│   │   │   ├── VideoMeet.jsx   # Video calling interface
│   │   │   ├── history.jsx     # Meeting history page
│   │   │   └── landing.jsx     # Landing page
│   │   ├── styles/
│   │   │   └── videoComponent.module.css # Video component styles
│   │   └── utils/
│   │       └── withAuth.jsx    # Authentication wrapper
│   ├── package.json            # Frontend dependencies
│   └── package-lock.json       # Dependency lock file
├── .gitignore                  # Git ignore file
└── README.md                   # This file
```

## Acknowledgments
* WebRTC technology for peer-to-peer video communication
* Socket.IO for real-time chat functionality
* Material UI for modern React components
* MongoDB Atlas for cloud database hosting
* Render for seamless deployment and hosting
* React community for excellent documentation and support

