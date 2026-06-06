# TaskFlow — Full Stack Task Management System

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

A full-stack task management application built with **NestJS**, **React**, and **MongoDB**. Features user authentication, Kanban-style task board, workspaces, comments, and real-time status updates.

---

## 🚀 Live Demo

- **Frontend:** [task-manager-nest.vercel.app](https://task-manager-nest.vercel.app) *(coming soon)*
- **Backend API:** [task-manager-nest-api.onrender.com](https://task-manager-nest-api.onrender.com) *(coming soon)*

---

## ✨ Features

- 🔐 **User Authentication** — Register, Login with JWT tokens
- 📋 **Task Management** — Create, edit, delete, and update tasks
- 🗂️ **Kanban Board** — Visual task board with Pending, In Progress, Completed columns
- 💬 **Comments** — Add comments and replies to tasks
- 🏢 **Workspaces** — Organize tasks by workspace
- 📊 **Dashboard Stats** — Live count of tasks by status
- 📱 **Fully Responsive** — Works on mobile, tablet, and desktop

---

## 🛠️ Tech Stack

### Backend
| Technology | Purpose |
|------------|---------|
| NestJS | Node.js framework with TypeScript |
| MongoDB + Mongoose | Database and ODM |
| JWT + Passport | Authentication |
| @nestjs/config | Environment configuration |
| class-validator | DTO validation |

### Frontend
| Technology | Purpose |
|------------|---------|
| React (Vite) | UI framework |
| Tailwind CSS | Styling |
| Redux Toolkit | State management |
| Axios | API calls |
| React Router | Navigation |
| Lucide React | Icons |

---

## 📁 Project Structure

```
task-manager-nest/
├── server/                    # NestJS Backend
│   └── src/
│       ├── auth/              # Authentication (JWT)
│       ├── tasks/             # Task CRUD
│       ├── workspace/         # Workspace management
│       ├── comments/          # Comments & replies
│       ├── app.module.ts      # Root module
│       └── main.ts            # Entry point
│
└── client/                    # React Frontend
    └── src/
        ├── api/               # Axios API calls
        ├── components/        # Reusable UI components
        ├── pages/             # Page components
        ├── store/             # Redux store
        └── App.jsx            # Root component
```

---

## ⚙️ Getting Started

### Prerequisites
- Node.js v18+
- MongoDB Atlas account
- npm

### 1. Clone the repository
```bash
git clone https://github.com/Afrafayas/task-manager-nest.git
cd task-manager-nest
```

### 2. Setup Backend
```bash
cd server
npm install
```

Create `.env` file in `server/`:
```env
PORT=5001
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.xxxxx.mongodb.net/taskmanager
JWT_SECRET=your_jwt_secret_key
```

Run the server:
```bash
npm run start:dev
```

Server runs on → `http://localhost:5001`

### 3. Setup Frontend
```bash
cd client
npm install
```

Create `.env` file in `client/`:
```env
VITE_API_URL=http://localhost:5001
```

Run the client:
```bash
npm run dev
```

Frontend runs on → `http://localhost:5173`

---

## 🔌 API Endpoints

### Auth
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register new user |
| POST | `/api/auth/login` | Login and get JWT token |

### Tasks
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/tasks` | Get all tasks |
| POST | `/api/tasks` | Create new task |
| PUT | `/api/tasks/:id` | Update task |
| DELETE | `/api/tasks/:id` | Delete task |

### Comments
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/tasks/:taskId/comments` | Add comment |
| DELETE | `/api/tasks/:taskId/comments/:commentId` | Delete comment |

### Workspace
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/workspace` | Get workspaces |
| POST | `/api/workspace` | Create workspace |

---

## 🚢 Deployment

- **Backend** deployed on [Render](https://render.com)
- **Frontend** deployed on [Vercel](https://vercel.com)

---

## 👩‍💻 Author

**Afra Fayas**
- GitHub: [@Afrafayas](https://github.com/Afrafayas)
- LinkedIn: [afra-fayas](https://linkedin.com/in/afra-fayas-aaa778246)

---

## 📄 Related Projects

- [task-manager](https://github.com/Afrafayas/task-manager) — MERN Stack Task Manager with Express + Redux

---

⭐ If you found this helpful, please give it a star!
