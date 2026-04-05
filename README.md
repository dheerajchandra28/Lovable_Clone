# 🚀 Dheeraj.dev — AI-Powered Web App Builder

Dheeraj.dev is a full-stack AI-powered platform that allows users to generate complete web applications using natural language prompts.

Instead of manually writing HTML, CSS, and JavaScript, users can simply describe what they want — and the system generates a fully functional web app with live preview and editable code.

---

## 🖼️ Preview
<p align="center">
  <img src="https://res.cloudinary.com/dulmeinq0/image/upload/v1775400094/Screenshot_2026-04-05_193634_l6lb7d.png" width="30%" />
  <img src="https://res.cloudinary.com/dulmeinq0/image/upload/v1775400080/Screenshot_2026-04-05_200052_ycdgpe.png" width="30%" />
  <img src="https://res.cloudinary.com/dulmeinq0/image/upload/v1775400080/Screenshot_2026-04-05_200035_w4v9x5.png" width="30%" />
</p>
---

## ✨ Features

### 🔐 Authentication

* User registration & login
* Secure password hashing using bcrypt
* JWT-based authentication
* Persistent login via cookies

### 📁 Project Management

* Create, view, rename, and delete projects
* Stores:

  * Chat history
  * Generated code
  * Version history

### 🤖 AI Code Generation

* Generate full HTML + CSS + JS apps using Gemini AI
* Iterative refinement via chat
* Context-aware responses

### 💬 Chat Interface

* Conversational UI
* Real-time AI responses
* Per-project message history

### 🖥️ Live Preview

* Instant rendering in iframe
* Secure sandbox execution

### 🧑‍💻 Code Editor

* Edit generated code
* Clean dark UI

### 📦 Download Feature

* Export project as standalone HTML

---

## 🏗️ Tech Stack

### Frontend

* React (Vite)
* React Router
* Axios
* Context API
* Custom CSS

### Backend

* Node.js
* Express.js
* MongoDB (Mongoose)
* JWT Authentication
* bcryptjs

### AI Integration

* Google Gemini API (`@google/genai`)
* Model: `gemini-2.5-flash`

---

## 📂 Project Structure

```
build-your-own-lovable/
│
├── server/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   └── constants/
│   └── server.js
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── services/
│   │   └── styles/
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone <your-repo-url>
cd build-your-own-lovable
```

### 2️⃣ Setup Backend

```bash
cd server
npm install
```

Create `.env` file:

```env
MONGODB_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
GEMINI_API_KEY=your_gemini_api_key
```

Run server:

```bash
npm run dev
```

---

### 3️⃣ Setup Frontend

```bash
cd client
npm install
npm run dev
```

---

## 🔗 API Endpoints

### Auth

* POST `/api/auth/register`
* POST `/api/auth/login`
* GET `/api/auth/me`
* POST `/api/auth/logout`

### Projects

* GET `/api/projects`
* POST `/api/projects`
* GET `/api/projects/:id`
* PUT `/api/projects/:id`
* DELETE `/api/projects/:id`

### AI Generation

* POST `/api/generate/:projectId`

---

## 💡 Future Improvements

* Version history UI with restore feature
* Public shareable project links
* Prompt templates library
* Multi-file code generation (React apps, etc.)

---

## 👨‍💻 Author

**Dheeraj.dev**
Building AI-powered developer tools 🚀

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
