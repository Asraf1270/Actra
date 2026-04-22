# 🚀 Actra — Personal Daily Activity Tracker

> **«Build consistency. Track your day. Improve your life.»**

Actra is a modern daily activity & habit tracking web app that helps users stay consistent, measure progress, and build better routines.

---

## ✨ Features

### 🧱 MVP Features

- 🔐 Authentication (Register / Login)
- 📝 Create, update, delete activities
- 📅 Daily activity tracking
- ✅ Mark tasks as completed
- 📊 Progress tracking (daily completion %)
- 📱 Responsive design (mobile-friendly)

---

## 🔥 Upcoming Features

- 🔥 Streak tracking system
- 📅 Calendar view
- 📊 GitHub-style heatmap
- 📈 Analytics dashboard
- 🔔 Notifications (PWA)
- 📧 Email reports
- 🎯 Goal setting
- 🧠 Smart insights
- 🌙 Dark mode

---

## 🛠 Tech Stack

### Frontend
- React (Vite)
- Axios
- React Router

### Backend
- Node.js (Express)
- JWT Authentication
- REST API

### Database
- PostgreSQL

---

## 📁 Project Structure

```
actra/
│
├── client/          # React frontend
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── services/
│
├── server/          # Node.js backend
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   └── config/
│
└── README.md
```

---

## ⚙️ Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/actra.git
cd actra
```

---

### 2️⃣ Setup Backend

```bash
cd server
npm install
```

Create a `.env` file:

```env
PORT=5000
DATABASE_URL=your_postgresql_connection
JWT_SECRET=your_secret_key
```

Run the server:

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

## 🗄 Database Schema (MVP)

### `users`
| Column | Type |
|---|---|
| id | UUID / Serial |
| name | VARCHAR |
| email | VARCHAR |
| password_hash | VARCHAR |
| created_at | TIMESTAMP |

### `activities`
| Column | Type |
|---|---|
| id | UUID / Serial |
| user_id | FK → users |
| title | VARCHAR |
| category | VARCHAR |
| created_at | TIMESTAMP |

### `activity_logs`
| Column | Type |
|---|---|
| id | UUID / Serial |
| activity_id | FK → activities |
| date | DATE |
| status | VARCHAR |

---

## 🔗 API Overview

### Auth
| Method | Endpoint |
|---|---|
| POST | `/api/auth/register` |
| POST | `/api/auth/login` |

### Activities
| Method | Endpoint |
|---|---|
| GET | `/api/activities` |
| POST | `/api/activities` |
| PUT | `/api/activities/:id` |
| DELETE | `/api/activities/:id` |

### Logs
| Method | Endpoint |
|---|---|
| POST | `/api/logs` |
| GET | `/api/logs/today` |

---

## 🎯 Vision

Actra is designed to evolve into a complete productivity system, not just a tracker.

**Future direction:**
- Data-driven insights
- Behavior analysis
- Smart habit optimization

---

## 🤝 Contributing

Contributions, ideas, and feedback are welcome!

1. Fork the repo
2. Create a new branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 💡 Inspiration

Built to combine:

- Simplicity of modern productivity tools
- Consistency tracking like developer workflows
- Clean and minimal UI experience

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---

> *«Small actions every day build extraordinary results.»*
