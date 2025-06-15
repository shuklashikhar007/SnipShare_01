# 🚀 Snip Share - Real-Time Collaborative Code Editor

Snip Share is a full-stack **real-time collaborative code editor** that enables multiple users to write, edit, and share code simultaneously. Whether you're doing pair programming, conducting interviews, or just want to share code snippets with friends — Snip Share has you covered!

## 🌐 Live Demo

> 🎥 **Demo Video:**  
[![Watch the video](assets/video-thumbnail.png)](VideoDemo-SnipShare.mp4)
  
---

## ✨ Features

- 🔗 Real-time collaboration with WebSockets
- ✍️ Code editor with syntax highlighting (powered by CodeMirror)
- 🧠 Multi-user support with live presence display
- 🚪 Room creation and joining via unique Room IDs
- 🧹 Code copy to clipboard
- 💬 User-friendly notifications using `react-hot-toast`
- 🔒 Unique user identification using UUID
- ⚡ Clean and responsive UI

---

<h1>Project Structure -> </h1>
<pre>
<code>
SnipShare_01/
├── client/
│   ├── public/
│   └── src/
│       ├── components/
│       │   ├── Client.js             # Component to show connected users
│       │   └── Editor.js             # Code editor using CodeMirror
│       ├── pages/
│       │   └── EditorPage.js         # Editor room interface with socket logic
│       ├── socket/
│       │   └── index.js              # Client-side socket setup
│       ├── Actions.js                # Socket action constants
│       ├── App.css                   # Styling for the frontend
│       ├── App.js                    # Root React component
│       └── index.js                  # Entry point for React app
├── server/
│   └── server.js                     # WebSocket server using Express and Socket.IO
├── package.json                      # Root project manifest
├── README.md                         # Project documentation
└── .gitignore
</code>
</pre>


---

## 🔧 How It Works

### 🧑‍💻 Join or Create a Room
- Landing page allows users to **enter a room ID** or generate a new one using UUID.
- Room ID is used to sync code across users.

### ✏️ Real-Time Editor
- Built using **CodeMirror 6**, it supports syntax highlighting, auto-indent, and keyboard shortcuts.
- All edits are instantly synced to connected clients.

### 🧑‍🤝‍🧑 Multi-user View
- Connected users are displayed via the `Client` component.
- Avatar and socket-based name sharing keeps everyone in sync.

### 📡 Socket.io WebSocket Communication
- Fast bi-directional data transfer between users.
- Supports real-time events like:
  - Code changes
  - New user joins
  - Disconnections

### 🔔 Notifications
- Seamless UI feedback using `react-hot-toast`.

---

## 🛠️ Built With

### Frontend
- **React** – UI framework
- **CodeMirror 6** – Rich text/code editor
- **React Router** – Routing between pages
- **React Hot Toast** – In-app notifications
- **UUID** – Unique Room ID generator
- **Socket.IO-client** – Real-time communication

### Backend
- **Node.js**
- **Socket.IO** – WebSocket server for real-time code collaboration
- **Express** – Lightweight HTTP server

---

## 📦 Packages & Dependencies

```bash
# Client Side
"react": "^18.x",
"react-dom": "^18.x",
"react-router-dom": "^6.x",
"react-hot-toast": "^2.x",
"uuid": "^9.x",
"codemirror": "^6.x",
"@codemirror/lang-javascript": "^6.x",
"@codemirror/theme-one-dark": "^6.x",
"socket.io-client": "^4.x"

# Server Side
"express": "^4.x",
"socket.io": "^4.x"

🧑‍🎓 Credits -
This project proudly uses and extends the following open-source packages:

react

codemirror

uuid

react-hot-toast

socket.io

express

react-router-dom



