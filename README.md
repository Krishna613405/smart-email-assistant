# 📧 Smart Email Assistant

> An AI-powered Email Assistant that helps users generate professional, context-aware email replies in seconds. Built using **Spring Boot**, **React**, and a **Chrome Extension**, this project integrates directly with Gmail to simplify email communication.

![Java](https://img.shields.io/badge/Java-21-orange)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-brightgreen)
![React](https://img.shields.io/badge/React-19-blue)
![Chrome Extension](https://img.shields.io/badge/Chrome_Extension-Manifest_V3-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Overview

Writing email replies can be repetitive and time-consuming. **Smart Email Assistant** uses Artificial Intelligence to generate meaningful and professional email responses based on the original email content and the selected writing tone.

The application consists of three major components:

- **Spring Boot Backend** – Handles AI integration and reply generation.
- **React Frontend** – Provides a clean web interface for users.
- **Chrome Extension** – Integrates directly into Gmail, allowing AI-generated replies without leaving the inbox.

---

# ✨ Features

✅ AI-generated email replies

✅ Multiple writing tones
- Professional
- Friendly
- Formal
- Casual

✅ Gmail integration using Chrome Extension

✅ Modern React interface

✅ RESTful Spring Boot API

✅ Responsive UI

✅ Fast AI response generation

✅ Easy to extend and customize

---

# 🏛️ System Architecture

```
                    ┌─────────────────────┐
                    │      Gmail UI       │
                    └──────────┬──────────┘
                               │
                      Chrome Extension
                               │
                               ▼
                    Spring Boot REST API
                               │
                        AI Language Model
                               │
                               ▼
                    Generated Email Reply
                               │
          ┌────────────────────┴──────────────────┐
          ▼                                       ▼
   React Application                    Gmail Compose Box
```

---

# 📂 Project Structure

```
Smart-Email-Assistant
│
├── email-writer-sb/
│   ├── src/
│   ├── pom.xml
│   └── application.properties
│
├── email-writer-react/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── email-writer-ext/
│   ├── manifest.json
│   ├── content.js
│   ├── content.css
│   └── icons/
│
└── README.md
```

---

# 🚀 Tech Stack

## Backend

| Technology | Purpose |
|------------|---------|
| Java 21 | Programming Language |
| Spring Boot | REST API |
| Maven | Dependency Management |
| Spring Web | API Development |
| Lombok | Boilerplate Reduction |

---

## Frontend

| Technology | Purpose |
|------------|---------|
| React | User Interface |
| Vite | Development Environment |
| Material UI | UI Components |
| Axios | API Communication |

---

## Browser Extension

| Technology | Purpose |
|------------|---------|
| JavaScript | Extension Logic |
| HTML | UI |
| CSS | Styling |
| Manifest V3 | Chrome Extension |

---

# ⚙️ Workflow

1. User opens the React application or Gmail.
2. User enters or selects an email.
3. User chooses the desired tone.
4. Request is sent to the Spring Boot backend.
5. Backend communicates with the AI model.
6. AI generates a professional email reply.
7. Generated response is displayed in the React app or automatically inserted into Gmail.

---

# 📡 REST API

## Generate Email Reply

```
POST /api/email/generate
```

### Request

```json
{
  "emailContent": "Can we schedule a meeting tomorrow?",
  "tone": "Professional"
}
```

### Response

```json
{
    "reply":"Dear Sir,\n\nThank you for your email.\nI am available tomorrow for the meeting.\n\nKind Regards,"
}
```

---

# 💻 Installation Guide

## Clone Repository

```bash
git clone https://github.com/<username>/Smart-Email-Assistant.git
```

```
cd Smart-Email-Assistant
```

---

## Backend Setup

```
cd email-writer-sb
```

Install dependencies

```bash
mvn clean install
```

Run

```bash
mvn spring-boot:run
```

Runs on

```
http://localhost:8080
```

---

## Frontend Setup

```
cd email-writer-react
```

Install packages

```bash
npm install
```

Start application

```bash
npm run dev
```

Runs on

```
http://localhost:5173
```

---

## Chrome Extension Setup

1. Open Chrome
2. Visit

```
chrome://extensions
```

3. Enable **Developer Mode**

4. Click **Load unpacked**

5. Select

```
email-writer-ext
```

6. Open Gmail

7. Compose or Reply to an email

8. Click **AI Reply**

---

# 📷 Screenshots

## Home Page

> Add Screenshot Here

---

## AI Generated Reply

> Add Screenshot Here

---

## Gmail Integration

> Add Screenshot Here

---

# 🎯 Future Enhancements

- Gmail OAuth Authentication
- Email History
- AI Reply Regeneration
- Multiple AI Models
- Dark Mode
- Reply Length Selection
- Multi-language Support
- Voice-to-Email
- Email Summarization
- Grammar Improvement
- Email Templates

---

# 📚 What I Learned

During the development of this project, I gained hands-on experience with:

- Full Stack Development
- Spring Boot REST APIs
- React Component Architecture
- Axios API Integration
- Chrome Extension Development
- Gmail DOM Manipulation
- Client-Server Communication
- AI Integration
- Modern UI Design
- Maven Project Management

---

# 🤝 Contributing

Contributions are welcome!

If you have ideas to improve this project:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

Feel free to use, modify, and improve it for learning purposes.

---

# 👨‍💻 Author

**Krishna Arjariya**

📧 Email: your-email@example.com

💼 LinkedIn: https://linkedin.com/in/your-profile

🐙 GitHub: https://github.com/your-username

---

# 🌟 Show Your Support

If you found this project helpful, please ⭐ the repository and share it with others.

It motivates me to build more open-source projects.

---
