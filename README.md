# 🏦 Digital Fixed Deposit System

<p align="center">
  <strong>A secure, full-stack digital banking platform for managing Fixed Deposits — architected and developed by Priyanshu Mishra.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=flat-square&logo=springboot"/>
  <img src="https://img.shields.io/badge/Spring_Security-JWT-6DB33F?style=flat-square"/>
  <img src="https://img.shields.io/badge/OAuth2-Google-4285F4?style=flat-square&logo=google"/>
  <img src="https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql"/>
  <img src="https://img.shields.io/badge/Vue_3-TypeScript-4FC08D?style=flat-square&logo=vuedotjs"/>
</p>

---

## 📌 Overview

The **Digital Fixed Deposit System** is a modern, secure, full-stack banking application that enables users to digitally manage Fixed Deposits — from booking and automated interest computation to maturity processing and withdrawal handling.

This project reflects strong backend architecture principles, production-grade authentication mechanisms, and clean frontend integration.

---

# 🏗️ System Architecture

## 🔹 Backend (Spring Boot)

- RESTful API design
- Layered architecture (Controller → Service → Repository)
- JWT-based authentication (Access + Refresh tokens)
- Refresh token rotation strategy
- Google OAuth2 login integration
- OTP-based email verification
- Scheduled tasks (FD maturity processing & OTP cleanup)
- Role-Based Access Control (RBAC)
- Global exception handling
- Structured logging using SLF4J + Logback
- Clean separation of DTOs and entities

## 🔹 Frontend (Vue 3 + TypeScript)

- Component-driven architecture
- Vue Router with route guards
- Vuex for centralized state management
- Axios interceptors for secure API communication
- Modular service layer abstraction
- Responsive and modern UI design

---

# 🛠 Tech Stack

## 🔹 Backend
- Java 17
- Spring Boot
- Spring Security
- JWT (HS256)
- OAuth2 (Google)
- PostgreSQL 16
- Maven
- Lombok
- SLF4J + Logback

## 🔹 Frontend
- Vue 3
- TypeScript
- Vite
- Vuex
- Vue Router
- Axios
- Sass

---

# 🔐 Security Architecture

- JWT-based authentication (Access + Refresh tokens)
- HTTP-only cookie storage
- Secure refresh token rotation
- Google OAuth2 authentication flow
- BCrypt password hashing
- Account lockout after multiple failed attempts
- OTP email verification system
- Role-based access control
- CORS security configuration
- Centralized global exception handling

---

# 💰 Core Functionalities

## 👤 User Capabilities
- Register with OTP verification
- Secure login & logout
- Login using Google OAuth2
- Book Fixed Deposits
- View and filter FD portfolio
- Track maturity timeline
- View calculated interest projections
- Break FD with penalty preview
- View withdrawal history
- Raise and track support tickets
- Manage profile settings

## 🛡 Admin Capabilities
- View all Fixed Deposits
- Update FD lifecycle status
- Monitor upcoming maturities
- Manage support tickets
- View financial summaries and reporting insights

---

# 📁 Project Structure

```
Digital-Fixed-Deposit-System
│
├── backend
│   ├── controller
│   ├── service
│   ├── repository
│   ├── entity
│   ├── config
│   ├── dto
│   ├── exception
│   └── util
│
├── frontend
│   ├── components
│   ├── views
│   ├── services
│   ├── store
│   ├── router
│   └── utils
```

---

# 🚀 Quick Start

## 🔹 Prerequisites

- Java 17+
- Node.js 18+
- PostgreSQL 16+
- Maven

---

## 🔹 Backend Setup

```bash
cd backend

# Configure application.properties:
# - Database credentials
# - JWT secret
# - Mail configuration
# - OAuth2 client credentials

./mvnw clean install
./mvnw spring-boot:run
```

Backend runs at:

```
http://localhost:8080
```

---

## 🔹 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at:

```
http://localhost:3000
```

---

# 🗄 Database Setup

Create PostgreSQL database:

```sql
CREATE DATABASE digital_fixed_deposit_system_db;
```

Update `application.properties`:

```
spring.datasource.url=jdbc:postgresql://localhost:5432/digital_fixed_deposit_system_db
spring.datasource.username=postgres
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

---

# 📊 Logging & Observability

- Structured logging using SLF4J
- Security event tracking
- Scheduler activity monitoring
- Centralized error handling via Global Exception Handler
- Application lifecycle logging

---

# 🎯 What This Project Demonstrates

- Secure authentication architecture (JWT + OAuth2)
- Token lifecycle management
- Financial business logic implementation
- Clean layered backend architecture
- RESTful API design principles
- State management in modern frontend frameworks
- Full-stack system integration
- Production-oriented coding practices

---

# 👨‍💻 Author

**Priyanshu Mishra**  
Full-stack developer focused on building secure, scalable backend systems and modern frontend applications.

---

# 📄 License

This project is licensed under the **MIT License**.

---

<p align="center">Built with ❤️ by Priyanshu Mishra</p>
