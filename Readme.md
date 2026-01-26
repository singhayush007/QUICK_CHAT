# 💬 QUICKCHAT — Real-Time Chat Application (MERN Stack + Socket.IO)

![QuickChat Screenshot](./client/src/assets/quickchat.png)

QUICKCHAT is a **full-stack MERN real-time chat application** that enables users to communicate instantly using Socket.IO.
It provides secure authentication, real-time messaging, and a modern responsive UI similar to popular chat platforms.
Users can register, log in, send and receive messages instantly without refreshing the page, and manage their profiles efficiently.

---

## 🧠 Features

- 🔐 User Authentication: Secure login & signup using JWT
- 💬 Real-Time Messaging: Instant message delivery with Socket.IO
- 🟢 Live Communication: No page reload required
- 👤 User Profiles: View and manage user profile information
- 📩 Message Persistence: Messages stored securely in MongoDB
- 💻 Responsive UI: Built using React and Tailwind CSS
- 📦 MongoDB Database: Store users and chat messages
- ⚡ Express.js Backend: REST APIs with middleware protection

---

## 💻 Tech Stack

| Technology                                                                                                       | Description                              |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| ![React.js](https://img.shields.io/badge/React.js-61DAFB?style=flat\&logo=react\&logoColor=black)                | Frontend library for building dynamic UI |
| ![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat\&logo=reactrouter\&logoColor=white)  | Client-side routing                      |
| ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat\&logo=tailwind-css\&logoColor=white) | Responsive UI design                     |
| ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat\&logo=node.js\&logoColor=white)                | Backend runtime                          |
| ![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat\&logo=express\&logoColor=white)          | Backend web framework                    |
| ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat\&logo=mongodb\&logoColor=white)                | NoSQL database                           |
| ![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat\&logo=mongoose\&logoColor=white)             | ODM for MongoDB                          |
| ![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=flat\&logo=socketdotio\&logoColor=white)        | Real-time communication                  |
| ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat\&logo=axios\&logoColor=white)                      | HTTP client                              |
| ![JWT](https://img.shields.io/badge/JWT-000000?style=flat\&logo=jsonwebtokens\&logoColor=white)                  | Authentication                           |
| ![Bcrypt](https://img.shields.io/badge/Bcrypt-3385FF?style=flat)                                                 | Password hashing                         |
| ![Cloudinary](https://img.shields.io/badge/Cloudinary-2B73B6?style=flat)                                         | Media storage                            |
| ![CORS](https://img.shields.io/badge/CORS-FFB400?style=flat)                                                     | Cross-origin handling                    |
| ![Nodemon](https://img.shields.io/badge/Nodemon-76D04B?style=flat)                                               | Dev server auto-restart                  |

---

## 🚀 Application Capabilities

| Feature                    | Description                                                    |
| -------------------------- | -------------------------------------------------------------- |
| 🔐 **Authentication**      | Secure JWT-based user authentication                           |
| 💬 **Real-Time Chat**      | Instant messaging using Socket.IO                              |
| 📩 **Message Storage**     | Messages saved in MongoDB                                      |
| 👤 **User Management**     | Profile viewing and updates                                    |
| 💻 **Responsive Frontend** | Clean UI using **React + Tailwind CSS**                        |
| ⚡ **Express Backend**      | REST APIs with controllers & middleware                        |
| 🌐 **Env Configuration**   | Secure environment variables using `.env`                      |
| ☁️ **Deployment Ready**    | Ready for deployment on **Vercel**, **Render**, or **Railway** |

---

## 🗂️ Folder Structure

```
QuickChat-Full-Stack/
│
├── client/                     # React + Vite frontend
│   ├── src/
│   │   ├── assets/             # Images & icons
│   │   ├── components/         # UI components
│   │   ├── pages/              # App pages
│   │   ├── lib/                # Utility functions
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── server/                     # Node.js + Express backend
│   ├── controllers/            # Business logic
│   ├── models/                 # MongoDB models
│   ├── routes/                 # API routes
│   ├── middleware/             # Auth middleware
│   ├── lib/                    # DB & helper configs
│   └── server.js               # Main server file
│
└── README.md
```

## 🏁 Getting Started

Follow these steps to run the project locally:

1. **Clone the repository**

```

git clone https://github.com/singhayush007/QUICK_CHAT.git
```

2. **Navigate to the project folder:**

```
cd QuickChat
```

3. **Install dependencies:**

```
npm install
```

4. **Create a .env.local file in the root and add your environment variables:**

```
PORT = ""
JWT_SECRET=""

# MongoDB URI
MONGODB_URI=your_mongodb_connection_uri

# Cloudinary Setup ( required )
CLOUDINARY_NAME = "your_cloud_name"
CLOUDINARY_API_KEY = "your_cloudinary_api_key"
CLOUDINARY_SECRET_KEY = "your_cloudinary_secret_key"
```

5. **Run the development server and client:**

```
cd client : npm run dev
cd server : npm run server
```

6. **Open the app in your browser:**

```
http://localhost:5173
```

## 💻 Deployment

You can deploy this app using Vercel, Docker, or any Node.js hosting platform.

## 📄 License

This project is licensed under the MIT License — feel free to use and modify it as per your needs.
