# 💬 ChatCord - Real-Time Chat Application

ChatCord is a real-time chat application built with **Node.js**, **Express**, and **Socket.io**. It allows multiple users to join specific chat rooms and exchange messages instantly with others in the same room.

## 🚀 Features

- Join chat rooms with a custom username  
- Real-time messaging using WebSockets  
- Welcome and disconnect messages  
- Shows current users in the room  
- Clean and responsive front-end using plain HTML/CSS/JS  

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js, Socket.io  
- **Frontend**: HTML, CSS, JavaScript  
- **Other**: dotenv for environment configuration  

## 📁 Project Structure

```
project/
│
├── public/                # Frontend files
│   ├── css/               # CSS styles
│   ├── js/                # Frontend socket logic
│   └── index.html         # Main HTML page
│
├── utils/
│   ├── messages.js        # Format chat messages
│   └── users.js           # Handle user join/leave/lookup
│
├── .env                   # Environment variables (PORT)
├── server.js              # Main server file
├── package.json
└── README.md
```

## 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/your-username/chatcord.git
cd chatcord
```

2. **Install dependencies**

```bash
npm install
```

3. **Run the server**

```bash
npm start
```

4. **Open in browser**

Visit: [http://localhost:3000](http://localhost:3000)

> Or change the port by editing the `.env` file:

```env
PORT=5000
```

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```
PORT=3000
```

## ✍️ How It Works

- The client connects to the server via Socket.io.  
- On joining a room, the server sends a welcome message to the user and broadcasts their arrival to others.  
- Messages are sent and received in real-time.  
- When a user leaves, the server notifies all other users in the same room.  

