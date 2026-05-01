# 🌐 Social Networking Platform

> A Full-Stack Social Media Web Application built from scratch using **Java Spring Boot** (Backend) and **React** (Frontend) — with real-time chat, reels, stories, and much more.

![Java](https://img.shields.io/badge/Java-17-orange?style=for-the-badge&logo=java)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0-green?style=for-the-badge&logo=springboot)
![React](https://img.shields.io/badge/React-18-blue?style=for-the-badge&logo=react)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?style=for-the-badge&logo=mysql)
![JWT](https://img.shields.io/badge/JWT-Auth-red?style=for-the-badge&logo=jsonwebtokens)

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔐 **User Authentication** | Secure JWT-based login & registration |
| 📰 **Posts & Feed** | Create, edit, and delete posts |
| 💬 **Comments & Likes** | Engage with posts |
| 📖 **Stories** | Short-lived 24-hour visual stories |
| 🎬 **Reels** | Upload and share short video clips |
| 👥 **Follow / Unfollow** | Follow other users for updates |
| 💬 **Real-time Chat** | WebSocket-powered live messaging |
| 👤 **Profile Page** | View and edit user profiles |

---

## 🛠️ Tech Stack

### Backend
- **Java 17** + **Spring Boot**
- **Spring Security** + **JWT** for authentication
- **Spring Data JPA** + **Hibernate**
- **WebSocket** for real-time communication
- **MySQL** as the database
- **Maven** as build tool
- **Lombok** to reduce boilerplate

### Frontend
- **React 18** + **Vite**
- **Redux Toolkit** for state management
- **Material UI (MUI)** for UI components
- **Tailwind CSS** for styling
- **Axios** for API calls
- **STOMP + SockJS** for WebSocket
- **Formik + Yup** for form validation

---

## 📁 Project Structure

```
Social-Networking-Platform/
├── springboot-social/          # Backend - Spring Boot
│   ├── src/
│   │   ├── main/java/com/.../
│   │   │   ├── controllers/    # REST Controllers
│   │   │   ├── services/       # Business Logic
│   │   │   ├── models/         # Entity Classes
│   │   │   ├── repositories/   # Database Layer
│   │   │   └── security/       # JWT & Auth
│   │   └── resources/
│   │       └── application.properties
│   └── pom.xml
│
└── client/                     # Frontend - React
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── redux/
    │   └── App.jsx
    └── package.json
```

---

## ⚙️ Getting Started

### Prerequisites
- Java 17+
- Node.js 18+
- MySQL 8.0+
- Maven 3.8+

### 🔧 Backend Setup

```bash
# 1. Navigate to backend folder
cd springboot-social

# 2. Configure MySQL in application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/socialdb
spring.datasource.username=your_username
spring.datasource.password=your_password

# 3. Run the backend
mvn spring-boot:run
```
Backend runs at: `http://localhost:8080`

### 💻 Frontend Setup

```bash
# 1. Navigate to frontend folder
cd client

# 2. Install dependencies
npm install

# 3. Start the frontend
npm run dev
```
Frontend runs at: `http://localhost:5173`

---

## 📡 API Endpoints

### Auth
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register new user |
| POST | `/api/auth/login` | Login & get JWT |

### Posts
| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/posts` | Get all posts |
| POST | `/api/posts` | Create a post |
| PUT | `/api/posts/{id}` | Edit a post |
| DELETE | `/api/posts/{id}` | Delete a post |

### Social
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/users/{id}/follow` | Follow a user |
| POST | `/api/users/{id}/unfollow` | Unfollow a user |
| POST | `/api/posts/{id}/like` | Like a post |
| POST | `/api/posts/{id}/comments` | Comment on a post |

### Reels & Stories
| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/reels` | Upload a reel |
| GET | `/api/reels` | Get all reels |
| POST | `/api/stories` | Create a story |
| GET | `/api/stories` | Get active stories |

---

## 🤝 Contributing

Contributions are welcome!

```bash
# Fork the repo, then:
git checkout -b feature/YourFeature
git commit -m "Add YourFeature"
git push origin feature/YourFeature
# Open a Pull Request
```

---

## 👨‍💻 Author

**Varun Kaushik**
- 🎓 B.Tech Engineering Student
- 💻 GitHub: [@curiousvarun](https://github.com/curiousvarun)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ **If you like this project, please give it a star — it motivates me to build more!**
