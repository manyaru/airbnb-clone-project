# airbnb-clone-project-BE

## 📖 About the Project

The **Airbnb Clone Project** is a real-world full-stack application designed to simulate the architecture, logic, and security of a scalable booking platform like Airbnb. It focuses heavily on backend systems, database design, API development, and secure deployment practices.

This project equips learners with in-depth experience in **software architecture**, **DevOps workflows**, and **collaborative development**, preparing them for large-scale production environments.

---

## 🎯 Learning Objectives

Through this project, you will:

- Master collaborative team workflows using GitHub
- Deepen your understanding of backend architecture and relational database design
- Implement secure RESTful APIs using Django and GraphQL
- Gain experience setting up CI/CD pipelines using tools like GitHub Actions and Docker
- Strengthen documentation and planning skills for full-stack applications
- Explore integration of modern technologies like **Django**, **MySQL**, and **GraphQL**

---

## ✅ Project Tasks Overview

| Task | Status | Description |
|------|--------|-------------|
| 0. Project Initialization | ✅ | Create GitHub repo & initial documentation |
| 1. Team Roles | ✅ | Define team roles and responsibilities |
| 2. Technology Stack | ✅ | List and explain core technologies used |
| 3. Database Design | ✅ | Outline entity relationships and key fields |
| 4. Feature Breakdown | ✅ | Describe core app features |
| 5. API Security | ✅ | Document key backend security measures |
| 6. CI/CD Pipeline | ✅ | Describe automated deployment process |

---

## 👥 Team Roles

| Role | Responsibility |
|------|----------------|
| **Backend Developer** | Builds APIs, handles logic, integrates DB |
| **Database Administrator** | Designs and manages relational database |
| **DevOps Engineer** | Implements CI/CD, manages containers and deployment |
| **QA Engineer** | Writes test cases, performs regression testing |
| **Documentation Lead** | Manages all written documentation |
| **Security Analyst** | Ensures backend security, performs audits |

Each role contributes to building a secure, scalable, and maintainable backend infrastructure.

---

## 💻 Technology Stack

| Technology | Purpose |
|------------|---------|
| **Django** | Backend web framework used to build REST and GraphQL APIs |
| **GraphQL** | Query language for flexible API interaction |
| **MySQL** | Relational database to store user, property, and booking data |
| **Docker** | Containerizes the app for consistent environments |
| **GitHub Actions** | Automates testing and deployment pipelines |
| **NGINX/Gunicorn** | Serves the production application securely and efficiently |

---

## 🗂️ Database Design

| Entity | Fields | Relationships |
|--------|--------|---------------|
| **User** | id, name, email, password, role | One user can own many properties and make many bookings |
| **Property** | id, title, description, location, price, user_id | Belongs to a user, has many bookings and reviews |
| **Booking** | id, user_id, property_id, start_date, end_date, status | Links a user to a property |
| **Review** | id, user_id, property_id, rating, comment | One review per booking, linked to user and property |
| **Payment** | id, booking_id, amount, status, timestamp | Linked to a booking |

> All relationships are built using **foreign keys** in a normalized relational structure. Indexes and constraints are enforced for performance and consistency.

---

## ⚙️ Feature Breakdown

### 👤 User Management
- Sign up, login, profile management
- Password encryption and role-based access

### 🏠 Property Management
- List, update, and delete user-owned properties
- Upload property photos and descriptions

### 📅 Booking System
- Search for properties by filters (location, price, availability)
- Make a booking with selected dates and number of guests

### 💳 Payment Integration
- Simulated or real payment gateway for bookings
- Payment success and failure handling

### ⭐ Review System
- Leave ratings and comments after stay
- See reviews per property

---

## 🔐 API Security

Security is central to this project. Key measures include:

| Area | Security Measures |
|------|-------------------|
| **Authentication** | JWT tokens for secure access to endpoints |
| **Authorization** | Role-based access (Admin, Host, Guest) |
| **Rate Limiting** | Prevent brute-force login attacks |
| **Input Validation** | Sanitize all data passed to the backend |
| **HTTPS** | Enforce secure data transfer during deployment |
| **CSRF Protection** | Ensures form integrity and protection against CSRF attacks |

> Security protects user data, financial info, and ensures system stability.

---

## 🔄 CI/CD Pipeline

CI/CD ensures efficient development and error-free deployments.

### 🛠️ What is CI/CD?
- **Continuous Integration (CI):** Automatically runs tests and builds on each push
- **Continuous Deployment (CD):** Automatically deploys to production after successful CI

### ⚙️ Tools Used:
- **GitHub Actions** – run tests, linting, and Docker builds
- **Docker** – containerize backend services and databases
- **Heroku / Render / Railway** – or any PaaS for deployment
- **PostgreSQL Add-On** – or linked DB container


