># COMPANY NAME : CODTECH IT SOLUTIONS PVT.LTD
># INTERN NAME  : KOTYADA JAHNAVI
># INTERN ID    : CT04DF2117
># DOMAIN       : FULL STACK WEB DEVELOPMENT
># DURATION     : 4 WEEKS
># MENTOR       : NEELA SANTHOSH


# OVERVIEW :

##  Real-Time Chat Application

###  Objective:


## ⚙ Technologies Used

| Layer     | Tech       | Purpose                               |
| --------- | ---------- | ------------------------------------- |
| Frontend  | HTML/CSS   | UI for chat box and messages          |
| Frontend  | JavaScript | Handles real-time messaging           |
| Backend   | Node.js    | Runs the server                       |
| Framework | Express.js | Serves static files (HTML, JS, CSS)   |
| WebSocket | Socket.IO  | Enables real-time 2-way communication |

---

##  Folder Structure

```
CT TASK2/
├── public/
│   ├── index.html     ← Chat UI
│   ├── style.css      ← Chat styling
│   └── script.js      ← Handles sending/receiving messages
├── server.js          ← Node.js + Socket.IO server
├── package.json       ← Project config & dependencies


##  How It Works (Step-by-Step)

1. **User opens the webpage (`index.html`)**
2. The page connects to the server using **Socket.IO**
3. When the user submits a message:

   * JavaScript sends the message using `socket.emit()`
4. The **Node.js server receives the message**

   * Then **broadcasts** it to all connected clients using `io.emit()`
5. All users see the new message instantly — **in real time**

---

## ▶Running the App

### Prerequisites:

* Node.js installed
* VS Code (or any IDE)

### Steps:

```bash
# 1. Create project folder & go inside
mkdir CT_TASK2 && cd CT_TASK2

# 2. Initialize Node.js project
npm init -y

# 3. Install dependencies
npm install express socket.io

# 4. Create folders/files: public/, index.html, script.js, style.css, server.js

# 5. Run the server
node server.js
```

### Open in Browser:

```bash
http://localhost:3000
```

Now you can chat between multiple tabs or devices!

---

##  Features You Can Add

* 👤 Usernames
* 🕒 Timestamps
* 📱 Mobile responsiveness
* 🎨 Themes or dark mode
* 🔐 Login system (with a database)

