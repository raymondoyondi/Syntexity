# 🚀 Syntexity

Syntexity is a powerful, real-time collaborative code and document editor built for developers who need to brainstorm, pair program, or draft documents together in an instant. By leveraging the MERN stack and WebSockets, Syntexity ensures that every keystroke is synchronized across all participants in a room.



## ✨ Features

* **Real-Time Collaboration:** Multiple users can edit the same file simultaneously with minimal latency.
* **Unique Room IDs:** Create private rooms and share the unique URL or ID with colleagues to start collaborating.
* **Live Cursor Tracking:** See who is typing and where they are in the document.
* **Syntax Highlighting:** Support for multiple programming languages to make code reviews easier.
* **Responsive Design:** Clean, minimalist UI built for both desktop and tablet views.

## 🛠️ Tech Stack

**Syntexity** is built using the **MERN** stack:

| Technology | Purpose |
| :--- | :--- |
| **MongoDB** | Database for storing persistent documents and user sessions. |
| **Express.js** | Backend framework for handling routing and API logic. |
| **React.js** | Frontend library for building the dynamic user interface. |
| **Node.js** | JavaScript runtime for the server-side environment. |
| **Socket.IO** | Enables real-time, bi-directional communication between clients and server. |

## 🚀 Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

* npm or yarn installed
* A MongoDB Atlas account or a local MongoDB instance

### Installation

1. **Clone the repository**
   ```bash
   git clone [https://github.com/raymondoyondi/Syntexity.git](https://github.com/raymondoyondi/Syntexity.git)
   cd Syntexity

2. **Install Backend Dependencies**
   ```
   cd server
   npm install
   ```
   
4. **Install Frontend Dependencies**
   ```
   cd ../client
   npm install
   ```
   
5. **Environment Setup**
Create a `.env` file in the `server` directory and add:
   ```
   REACT_APP_BACKEND_URL="http://localhost:5050"
   REACT_APP_clientId="jdoodle client id"
   REACT_APP_clientSecret="jdoodle client secret"
   MONGO_URL="mongodb uri"
   ```
   
6. **Run the Application**
Open two terminals:

- In `/server`: npm start
- In `/client`: npm start

## 📡 How it Works

Syntexity uses WebSockets (via Socket.io) to maintain a persistent connection. When a user modifies the text, a "change" event is emitted to the server, which then broadcasts that specific delta to all other users in the same Room ID.

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
