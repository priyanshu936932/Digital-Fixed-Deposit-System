# 🏦 Digital Fixed Deposit System

<p align="center">
  <strong>A full-stack banking application for managing Fixed Deposits digitally — designed and developed entirely by Priyanshu Mishra.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring_Boot-4.0-6DB33F?style=flat-square&logo=springboot"/>
  <img src="https://img.shields.io/badge/Spring_Security-JWT-6DB33F?style=flat-square"/>
  <img src="https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql"/>
  <img src="https://img.shields.io/badge/Vue_3-TypeScript-4FC08D?style=flat-square&logo=vuedotjs"/>
  <img src="https://img.shields.io/badge/Docker-Ready-2496ED?style=flat-square&logo=docker"/>
</p>

---

## 📌 Overview

The **Digital Fixed Deposit System** is a secure, full-stack banking platform that enables users to digitally manage Fixed Deposits — from booking to maturity and withdrawal.

This project demonstrates:

- Secure authentication and authorization
- Financial calculations with business rules
- Full-stack integration
- Scheduled background processing
- Clean layered architecture
- Logging and exception handling

---

# 🏗️ System Architecture

## 🔹 Backend (Spring Boot)

- RESTful API architecture
- Layered design (Controller → Service → Repository)
- JWT authentication (HTTP-only cookies)
- Google OAuth2 integration
- OTP-based email verification
- Scheduled tasks (FD maturity, OTP cleanup)
- Global exception handling
- Structured logging with SLF4J + Logback

## 🔹 Frontend (Vue 3 + TypeScript)

- Component-based architecture
- Vue Router with route guards
- Vuex state management
- Axios interceptors for authentication
- Modular service layer
- Responsive UI design

---

# 🛠 Tech Stack

## Backend
- Java 17
- Spring Boot 4
- Spring Security
- JWT (HS256)
- OAuth2 (Google)
- PostgreSQL
- Maven
- Lombok
- JUnit 5
- JaCoCo
- SLF4J + Logback Logging

## Frontend
- Vue 3
- TypeScript
- Vite
- Vuex
- Vue Router
- Axios
- Sass

---

# 🔐 Security Features

- JWT-based authentication (Access + Refresh tokens)
- Token rotation strategy
- HTTP-only cookie storage
- BCrypt password hashing
- Account lockout mechanism
- OTP email verification
- Role-based access control
- Global exception handling
- CORS configuration

---

# 💰 Core Functionalities

## 👤 User Features
- Register with email OTP verification
- Secure login and logout
- Google OAuth2 login
- Book Fixed Deposits
- View and filter FDs
- Track maturity dates
- Interest timeline view
- Break FD with penalty preview
- View withdrawal history
- Raise support tickets
- Profile management

## 🛡 Admin Features
- View all FDs
- Update FD status
- Monitor maturing FDs
- Manage support tickets
- Financial summaries and reports

---

# 📁 Project Structure


Digital-Fixed-Deposit-System
│
├── backend
│ ├── controller
│ ├── service
│ ├── repository
│ ├── entity
│ ├── config
│ ├── dto
│ ├── exception
│ └── util
│
├── frontend
│ ├── components
│ ├── views
│ ├── services
│ ├── store
│ ├── router
│ └── utils


---

# 🚀 Quick Start

## 🔹 Prerequisites

- Java 17+
- Node.js 18+
- PostgreSQL 16+
- Maven
- Docker (optional)

---

## 🔹 Backend Setup

```bash
cd backend

# Configure application.properties
# Set database, JWT secret, mail credentials, OAuth2 credentials

./mvnw clean install
./mvnw spring-boot:run

Backend runs at:

http://localhost:8080
🔹 Frontend Setup
cd frontend
npm install
npm run dev

Frontend runs at:

http://localhost:3000
🗄 Database

Create PostgreSQL database:

CREATE DATABASE Digital_Fixed_Deposit_System_DB;

Update application.properties:

spring.datasource.url=jdbc:postgresql://localhost:5432/Digital_Fixed_Deposit_System_DB
spring.datasource.username=postgres
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
🐳 Docker Deployment (Optional)
docker build -t digital-fd-backend ./backend
docker build -t digital-fd-frontend ./frontend
docker-compose up -d
🧪 Testing
Backend
./mvnw test
./mvnw clean test jacoco:report

Coverage report:

target/site/jacoco/index.html
Frontend
npm run test
npm run coverage
📊 Logging

Structured logging using SLF4J

Application startup logs

Security event logs

Error logs via Global Exception Handler

Scheduler activity logs

🎯 Learning Outcomes

This project demonstrates:

Secure authentication architecture

Financial business logic implementation

Clean layered backend design

Full-stack integration

Token-based security

State management in frontend

REST API development

Production-ready logging

👨‍💻 Author

Priyanshu Mishra

Full-stack developer focused on building secure, scalable backend systems and modern frontend applications.

📄 License

This project is licensed under the MIT License.

<p align="center"> Built with ❤️ by Priyanshu Mishra </p> ```