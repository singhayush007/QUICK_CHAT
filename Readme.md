# 💬 QuickChat — Real-Time Chat Application

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/singhayush007/QUICK_CHAT?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/singhayush007/QUICK_CHAT?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/singhayush007/QUICK_CHAT?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Made with MERN](https://img.shields.io/badge/Stack-MERN-61DAFB?style=flat-square&logo=react&logoColor=black)

**A production-ready full-stack real-time chat application built with the MERN stack and Socket.IO.**

[🌐 Live Demo](https://quickchat-mern.vercel.app) · [🐛 Report Bug](https://github.com/singhayush007/QUICK_CHAT/issues) · [✨ Request Feature](https://github.com/singhayush007/QUICK_CHAT/issues)

</div>

---

![QuickChat Screenshot](./client/src/assets/quickchat.png)

---

## 📋 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Folder Structure](#️-folder-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Running the App](#️-running-the-app)
- [Deployment](#️-deployment)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📖 About

**QuickChat** is a full-stack MERN real-time chat application that enables users to communicate instantly using **Socket.IO** — no page refresh required.

- **Users** can register, log in, and manage their profiles with avatar uploads.
- **Real-time messaging** is delivered instantly across all connected clients.
- **Messages are persisted** in MongoDB so chat history is always available.

---

## ✨ Features

| Feature | Description |
| --- | --- |
| 🔐 **JWT Authentication** | Secure login & signup with token-based auth stored in HTTP-only cookies |
| 💬 **Real-Time Messaging** | Instant message delivery powered by **Socket.IO** |
| 🟢 **Online Status** | See which users are currently online in real time |
| 👤 **User Profiles** | View and update profile info with avatar image support |
| 📩 **Message Persistence** | All messages are stored securely in **MongoDB** |
| ☁️ **Image Uploads** | Profile picture uploads via **Cloudinary** |
| 💻 **Responsive UI** | Clean, mobile-friendly UI built with **React.js** and **Tailwind CSS** |
| 🔒 **Secure Backend** | Password hashing with **Bcrypt**, CORS protection, and auth middleware |
| 🌐 **Deployment Ready** | Configured for **Vercel**, **Render**, or **Railway** |

---

## 💻 Tech Stack

### Frontend
![React.js](https://img.shields.io/badge/React.js-61DAFB?style=flat&logo=react&logoColor=black)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat&logo=reactrouter&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwind-css&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat&logo=axios&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-orange?style=flat)
![Socket.IO Client](https://img.shields.io/badge/Socket.IO_Client-010101?style=flat&logo=socketdotio&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat)
![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat&logo=socketdotio&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![Bcrypt](https://img.shields.io/badge/Bcrypt-3385FF?style=flat)
![Cloudinary](https://img.shields.io/badge/Cloudinary-2B73B6?style=flat)
![Nodemon](https://img.shields.io/badge/Nodemon-76D04B?style=flat)

---

## 🗂️ Folder Structure

```
QuickChat-Full-Stack/
│
├── client/                     # React + Vite frontend
│   ├── src/
│   │   ├── assets/             # Images & icons
│   │   ├── components/         # Reusable UI components
│   │   ├── context/            # React context providers
│   │   ├── lib/                # Utility functions & helpers
│   │   ├── pages/              # App pages (Login, Chat, Profile)
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── .env                    # Local env (not committed)
│   ├── .env.example            # Env template
│   ├── package.json
│   └── vite.config.js
│
├── server/                     # Node.js + Express backend
│   ├── controllers/            # Route controllers (auth, message, user)
│   ├── models/                 # Mongoose models (User, Message)
│   ├── routes/                 # API route definitions
│   ├── middleware/             # Auth middleware
│   ├── lib/                    # DB connection, Cloudinary, Socket config
│   ├── .env                    # Local env (not committed)
│   ├── .env.example            # Env template
│   └── server.js               # Main server entry point
│
└── Readme.md
```

---

## 🏁 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) v18+
- [npm](https://www.npmjs.com/) v9+
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) account (or local MongoDB)
- [Cloudinary](https://cloudinary.com/) account

### 1. Clone the repository

```bash
git clone https://github.com/singhayush007/QUICK_CHAT.git
cd QUICK_CHAT
```

### 2. Install dependencies

The client and server each have their own `package.json`. Install them separately:

```bash
# Server
cd server && npm install

# Client
cd ../client && npm install
```

---

## 🔐 Environment Variables

Each package has a `.env.example` file. Copy it to `.env` and fill in your values.

### Server (`server/.env`)

```bash
cp server/.env.example server/.env
```

| Variable | Description |
| --- | --- |
| `PORT` | Port the server runs on (default: `5000`) |
| `JWT_SECRET` | Secret key for signing JWT tokens |
| `MONGODB_URI` | MongoDB connection string |
| `CLOUDINARY_CLOUD_NAME` | Cloudinary cloud name |
| `CLOUDINARY_API_KEY` | Cloudinary API key |
| `CLOUDINARY_API_SECRET` | Cloudinary API secret |

### Client (`client/.env`)

```bash
cp client/.env.example client/.env
```

| Variable | Description |
| --- | --- |
| `VITE_BACKEND_URL` | Backend API base URL (e.g. `http://localhost:5000`) |

---

## ▶️ Running the App

Open **two separate terminals** and run:

```bash
# Terminal 1 — Backend (runs on http://localhost:5000)
cd server
npm run server
```

```bash
# Terminal 2 — Frontend (runs on http://localhost:5173)
cd client
npm run dev
```

Then open [http://localhost:5173](http://localhost:5173) in your browser.

---

## ☁️ Deployment

This project is ready to deploy on modern cloud platforms.

| Service | Recommended For |
| --- | --- |
| [Vercel](https://vercel.com) | Frontend (React + Vite) |
| [Render](https://render.com) | Backend (Node.js + Express) |
| [Railway](https://railway.app) | Backend (Node.js + Express) |
| [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) | Database |
| [Cloudinary](https://cloudinary.com) | Media / Image Storage |

> Make sure to set all environment variables in your hosting platform's dashboard before deploying.

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'add: your feature description'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use and modify it as per your needs.

---

<div align="center">
  Made with ❤️ by <a href="https://github.com/singhayush007/QUICK_CHAT">Ayush Singh</a>
</div>
