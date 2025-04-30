🗳️ Electronic Voting System
This project is a real-time electronic voting system built with Node.js, Express, MongoDB, and Socket.io. It allows users to register and vote, with instant vote updates delivered via WebSockets.

🚀 Features
User authentication (via /api/auth)

Secure vote submission (via /api/vote)

Real-time vote count updates using Socket.io

MongoDB for persistent storage

CORS enabled for frontend access

Easy to set up and run

🛠️ Tech Stack
Backend: Node.js, Express.js, MongoDB, Mongoose

Real-time Communication: Socket.io

Environment Management: dotenv

Frontend: (Assuming you’re using a frontend like React on port 5173)

⚙️ Installation and Setup

1.  Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2.  Install dependencies

```bash
npm install
```

3.  Set up your .env file Create a .env file in the root directory and add:

```ini
MONGO_URI=your_mongo_connection_string
PORT=7777
```

4.  Run the server

```bash
node server.js
```
The server will run on: http://localhost:7777

5.  Frontend Setup (if applicable) Make sure your frontend (e.g., React app) runs on http://localhost:5173, or change the cors setting in server.js accordingly.

📡 Real-time Communication
When a user votes, a new-vote event is emitted via Socket.io.

All connected clients receive updated results through the vote-update event.

🔒 Security
Be sure to add authentication/authorization layers to protect your routes in a production version.

Make sure your MongoDB connection string in .env is never committed to the repository.

🧪 Sample API Endpoints
POST /api/auth/register – Register a user

POST /api/auth/login – Log in a user

POST /api/vote – Submit a vote

WebSocket events: new-vote, vote-update

🙌 Credits
Developed by Moulik Chakradhar
3rd Year CSE - Cyber Security







