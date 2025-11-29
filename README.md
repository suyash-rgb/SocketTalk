# SocketTalk 💬

## Project Overview
SocketTalk is a real-time chat application built with **Spring Boot** and **WebSockets**.  
It demonstrates how to implement bi-directional communication between clients and servers using STOMP over WebSocket, with a simple **Telegram-inspired frontend UI**.  

The goal of this project is to provide a clean, educational example of:
- Setting up a WebSocket backend in Java/Spring Boot
- Broadcasting messages to multiple participants
- Building a responsive frontend with HTML, CSS, and JavaScript
- Managing participants and aligning messages like modern chat apps

---

## Technologies Used
- **Backend**
  - Java 17+
  - Spring Boot (Web, WebSocket, Messaging)
  - STOMP over SockJS
- **Frontend**
  - HTML5
  - Inline CSS (Telegram-inspired design)
  - Vanilla JavaScript
  - SockJS Client
  - STOMP.js
- **Build Tools**
  - Maven (for dependency management and build)

---

## Prerequisites
Before running SocketTalk, ensure you have:
- **Java 17+** installed
- **Maven** installed
- A modern browser (Chrome/Firefox/Edge)
- Internet access (to load SockJS and STOMP.js from CDN)

---

## Installation (Backend + Frontend Setup)

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/SocketTalk.git
cd SocketTalk
```

### 2. Backend Setup
- Navigate to the backend project root.
- Build and run the Spring Boot application:

```bash
mvn spring-boot:run
```

### - The server will start on http://localhost:8080.
Spring Boot will expose:
- WebSocket endpoint: ```/ws```
- Message mapping: ```/app/sendMessage```
- Broadcast topic: ```/topic/messages```

