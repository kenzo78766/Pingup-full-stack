# 🌐 PingUp --- Full-Stack Social Media Platform

> A modern full-stack social media platform featuring real-time
> messaging, user connections, stories, posts, notifications, and
> cloud-based media management.

```{=html}
<p align="center">
```
`<a href="https://pingup-client-ashy-xi.vercel.app/">`{=html}`<img src="https://img.shields.io/badge/🚀%20LIVE%20DEMO-00C853?style=for-the-badge" />`{=html}`</a>`{=html}
`<a href="https://github.com/kenzo78766/Pingup-full-stack">`{=html}`<img src="https://img.shields.io/badge/💻%20SOURCE%20CODE-181717?style=for-the-badge&logo=github" />`{=html}`</a>`{=html}
```{=html}
</p>
```

------------------------------------------------------------------------

## ✨ Features

-   🔐 **Authentication & Account Management** --- Secure authentication
    with Clerk, profile management, persistent sessions, and
    multi-account switching.
-   📰 **Social Feed** --- Create posts with multiple images, view
    connected users' content, like posts, and manage published content.
-   👥 **Connections & User Discovery** --- Search users by name,
    username, bio, and location, send connection requests, and manage
    connections.
-   💬 **Real-Time Messaging** --- Chat between users in real time with
    unread-message tracking and notification support.
-   📖 **Stories** --- Create and view temporary stories with automatic
    expiration after 24 hours.
-   🔔 **Background Notifications** --- Inngest-powered workflows for
    connection-request reminders, unseen-message notifications, and
    scheduled tasks.
-   🖼️ **Cloud Media Management** --- ImageKit integration for profile
    pictures, post images, and story media.
-   👤 **Profile Management** --- Edit profiles, manage account
    information, and view posts, connections, media, and profile
    activity.

------------------------------------------------------------------------

## 📸 Project Preview

### 🏠 Feed & Home

![PingUp Feed](screenshots/feed.png)

### 👤 Profile

![PingUp Profile](screenshots/profile.png)

### 💬 Real-Time Messaging

![PingUp Messaging](screenshots/messages.png)

### 👥 Connections

![PingUp Connections](screenshots/connections.png)

### 📖 Stories

![PingUp Stories](screenshots/stories.png)

### 📝 Create Post

![PingUp Create Post](screenshots/create-post.png)

------------------------------------------------------------------------

## 🛠️ Tech Stack

### Frontend

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Tailwind
CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

### Backend

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

### Services & Cloud

![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge)
![ImageKit](https://img.shields.io/badge/ImageKit-00AEEF?style=for-the-badge)
![Inngest](https://img.shields.io/badge/Inngest-000000?style=for-the-badge)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

------------------------------------------------------------------------

## 🏗️ Application Architecture

``` text
                         ┌──────────────────┐
                         │      User        │
                         └────────┬─────────┘
                                  │
                                  ▼
                         ┌──────────────────┐
                         │ React Frontend   │
                         │  + Tailwind CSS  │
                         └────────┬─────────┘
                                  │
                              REST API
                                  │
                                  ▼
                         ┌──────────────────┐
                         │ Node.js/Express  │
                         │     Backend      │
                         └────────┬─────────┘
                                  │
             ┌────────────────────┼────────────────────┐
             │                    │                    │
             ▼                    ▼                    ▼
       ┌───────────┐       ┌───────────┐       ┌───────────┐
       │  MongoDB  │       │   Clerk   │       │  ImageKit │
       │   Atlas   │       │   Auth    │       │   Media   │
       └───────────┘       └───────────┘       └───────────┘
                                  │
                                  ▼
                           ┌────────────┐
                           │  Inngest   │
                           │ Background │
                           │  Workflows │
                           └────────────┘
```

------------------------------------------------------------------------

## 📂 Project Structure

``` text
PingUp/
├── client/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── app/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── features/
│   │   └── pages/
│   └── package.json
├── server/
│   ├── configs/
│   ├── controllers/
│   ├── inngest/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
├── screenshots/
└── README.md
```

------------------------------------------------------------------------

## ⚙️ Run Locally

### 1. Clone Repository

``` bash
git clone https://github.com/kenzo78766/Pingup-full-stack.git
cd Pingup-full-stack
```

### 2. Start Frontend

``` bash
cd client
npm install
npm run dev
```

### 3. Start Backend

``` bash
cd server
npm install
npm start
```

------------------------------------------------------------------------

## 🔑 Environment Variables

Create `.env` files for the frontend and backend and configure the
required credentials for MongoDB Atlas, Clerk, ImageKit, Inngest, the
email service, and frontend/backend URLs.

> ⚠️ Never commit `.env` files or secret credentials to GitHub.

------------------------------------------------------------------------

## 🚀 Deployment

  Component         Technology
  ----------------- ---------------
  Frontend          Vercel
  Backend           Vercel
  Database          MongoDB Atlas
  Authentication    Clerk
  Media Storage     ImageKit
  Background Jobs   Inngest
  Email Service     Nodemailer

------------------------------------------------------------------------

## 🎯 Key Learning Outcomes

-   Full-stack application development using React and Node.js.
-   REST API development and integration.
-   MongoDB database design and management.
-   Authentication and user management.
-   Real-time messaging workflows.
-   Cloud-based media handling.
-   Background job and scheduled task processing.
-   Third-party service integration.
-   Production deployment and environment configuration.

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Advanced content recommendation.
-   Enhanced privacy and account controls.
-   Improved real-time notification system.
-   Automated testing and CI/CD pipelines.
-   Application performance monitoring.

------------------------------------------------------------------------

## 👨‍💻 Author

### Anshuman Singh

[![GitHub](https://img.shields.io/badge/GitHub-kenzo78766-181717?style=for-the-badge&logo=github)](https://github.com/kenzo78766)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Anshuman%20Singh-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/anshuman78766)

------------------------------------------------------------------------

⭐ If you found this project useful, consider giving the repository a
star!
