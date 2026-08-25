# 🌐 PingUp — Full-Stack Social Media Platform

> A modern full-stack social media platform built for meaningful connections, real-time communication, content sharing, and a smooth social experience.

<p align="center">
  <a href="https://pingup-client-ashy-xi.vercel.app/">
    <img src="https://img.shields.io/badge/🚀%20LIVE%20DEMO-PingUp-5B3DF5?style=for-the-badge" alt="Live Demo">
  </a>
  <a href="https://github.com/kenzo78766/Pingup-full-stack">
    <img src="https://img.shields.io/badge/💻%20SOURCE%20CODE-GitHub-181717?style=for-the-badge&logo=github" alt="Source Code">
  </a>
  <a href="https://www.linkedin.com/in/anshuman78766/">
    <img src="https://img.shields.io/badge/LinkedIn-Anshuman%20Singh-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn">
  </a>
</p>

---

## ✨ Overview

**PingUp** is a full-stack social media application that combines social networking, content sharing, connections, notifications, and real-time messaging into one platform.

The application includes secure authentication, personalized profiles, a social feed, stories, post creation, connection management, discovery/search, and real-time one-to-one messaging.

---

## 🚀 Live Demo

🔗 **Live Application:** https://pingup-client-ashy-xi.vercel.app/

🔗 **GitHub Repository:** https://github.com/kenzo78766/Pingup-full-stack

🔗 **LinkedIn:** https://www.linkedin.com/in/anshuman78766/

---

## 🎯 Key Features

### 🔐 Authentication & Account Management
- Secure user authentication and sign-in flow powered by **Clerk**.
- User account management with profile information and session handling.
- Support for managing multiple accounts and switching between accounts.

### 🏠 Feed & Social Posts
- Personalized social feed for viewing posts from connected users.
- Create and publish posts with text content and multiple images.
- View post engagement including likes, comments, and shares.
- Delete and manage created posts.
- Hashtag support for posts.

### 📖 Stories
- Create and view user stories from the feed.
- Story content is designed around temporary social updates.
- Automated story deletion is handled using **Inngest** workflows.

### 👤 Profiles
- Dedicated user profile pages with:
  - Profile picture
  - Cover image
  - Bio
  - Location
  - Posts
  - Followers
  - Following
  - Media
  - Likes
- Edit profile information directly from the application.
- View another user's profile and social activity.

### 🤝 Connections
- Discover other users and send connection requests.
- Accept or manage incoming connection requests.
- Connection status is reflected throughout the application.
- Automated email reminders are triggered for pending connection requests.

### 🔎 Discover & Search
- Search and discover users using information such as:
  - Name
  - Username
  - Bio
  - Location
- Browse users and connect with people across the platform.

### 💬 Real-Time Messaging
- Real-time one-to-one chat between different user accounts.
- Send and receive messages without manually refreshing the page.
- Conversation interface for managing ongoing chats.
- Recent/unseen message information is surfaced through notifications.

### 🔔 Notifications & Automated Workflows
- Unseen-message notification system.
- Automated email notifications for connection requests.
- Scheduled background workflows using **Inngest**.
- Reminder workflows can check pending connection requests after a defined period.

### 🖼️ Media Management
- Support for image-based posts, profiles, and stories.
- Cloud-based media handling for uploaded content.

---

## 🛠️ Tech Stack

### Frontend
- **React.js**
- **Vite**
- **Tailwind CSS**
- **Clerk**

### Backend
- **Node.js**
- **Express.js**
- **MongoDB**
- **Mongoose**

### Real-Time & Background Processing
- **Inngest** — event-driven background jobs, scheduled workflows, and automated tasks.
- Real-time messaging architecture for live user-to-user communication.

### Services & Tools
- **Nodemailer** — transactional email notifications.
- **Git & GitHub** — version control and source management.
- **Vercel** — deployment and hosting.

---

## 📸 Application Preview

### 🔐 Login & Authentication

<p align="center">
  <a href="https://drive.google.com/file/d/1CMsOTqp5d0j2R144n7EH6tUT3GKbs8z7/view?usp=sharing">
    <img src="https://drive.google.com/uc?export=view&id=1CMsOTqp5d0j2R144n7EH6tUT3GKbs8z7" alt="PingUp Login & Authentication" width="900">
  </a>
</p>

### 🏠 Feed & Dashboard

<p align="center">
  <a href="https://drive.google.com/file/d/16G_Ula2wZtGIERojXNf54ruHgculHkqy/view?usp=sharing">
    <img src="https://drive.google.com/uc?export=view&id=16G_Ula2wZtGIERojXNf54ruHgculHkqy" alt="PingUp Dashboard" width="900">
  </a>
</p>

### 👤 User Profile

<p align="center">
  <a href="https://drive.google.com/file/d/1QmZqxxHOz-sJUSwI6NcwbnfqGYYfSfdH/view?usp=sharing">
    <img src="https://drive.google.com/uc?export=view&id=1QmZqxxHOz-sJUSwI6NcwbnfqGYYfSfdH" alt="PingUp User Profile" width="900">
  </a>
</p>

## 🏗️ Project Structure

```text
Pingup-full-stack/
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── assets/
│   │   └── ...
│   └── package.json
│
├── server/
│   ├── configs/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── inngest/
│   └── ...
│
└── README.md
```

---

## ⚙️ Core Backend Workflows

PingUp uses event-driven workflows to handle operations that should not block normal API requests.

Examples include:

- Synchronizing Clerk user creation, updates, and deletion with MongoDB.
- Sending connection-request emails.
- Sending reminder emails for pending connection requests.
- Automatically deleting expired stories.
- Sending scheduled notifications for unseen messages.

---

## 🔄 Application Flow

```text
User
 │
 ▼
React Frontend
 │
 ├── Authentication ───────► Clerk
 │
 ├── API Requests ────────► Express / Node.js
 │                              │
 │                              ▼
 │                          MongoDB
 │
 ├── Real-Time Chat ──────► Messaging Layer
 │
 └── Social Actions
        │
        ▼
   Posts / Stories / Connections
        │
        ▼
     Inngest
        │
        ├── Background Jobs
        ├── Scheduled Tasks
        └── Notifications / Emails
```

---

## 🧩 Main Modules

| Module | Description |
|---|---|
| Authentication | Secure sign-in and account/session management |
| Feed | Personalized posts and social interactions |
| Posts | Create, view, manage, and engage with posts |
| Stories | Temporary social updates with automated expiry |
| Profiles | User information, posts, media, and social statistics |
| Connections | Send, receive, accept, and manage connection requests |
| Discover | Search and discover users |
| Messaging | Real-time one-to-one conversations |
| Notifications | Unseen message and connection-related notifications |
| Background Jobs | Event-driven and scheduled workflows with Inngest |

---

## 🚀 Running Locally

### 1. Clone the repository

```bash
git clone https://github.com/kenzo78766/Pingup-full-stack.git
cd Pingup-full-stack
```

### 2. Install frontend dependencies

```bash
cd client
npm install
```

### 3. Install backend dependencies

```bash
cd ../server
npm install
```

### 4. Configure environment variables

Create the required `.env` files for the client and server and add your authentication, database, email, media, Inngest, and frontend configuration values.

### 5. Start the backend

```bash
cd server
npm run server
```

### 6. Start the frontend

```bash
cd client
npm run dev
```

---

## 🌍 Deployment

The application is deployed using **Vercel**, with the frontend and backend configured as separate deployment targets.

🔗 **Production Frontend:** https://pingup-client-ashy-xi.vercel.app/

---

## 👨‍💻 Developer

### Anshuman Singh

Computer Science Student & Full-Stack Developer

🔗 **LinkedIn:** https://www.linkedin.com/in/anshuman78766/

🔗 **GitHub:** https://github.com/kenzo78766

---

## ⭐ Project Highlights

- Full-stack social media architecture
- Secure authentication and account management
- Real-time user-to-user messaging
- Event-driven background processing
- Scheduled notifications and automated workflows
- Social connections and discovery
- Stories and multi-image posts
- Profile and account management
- Production deployment with Vercel
- Responsive, modern social-media-style interface

---

<p align="center">
  <b>PingUp — More than just friends, truly connect.</b>
</p>
