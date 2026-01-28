# Blu-Reserv — Restaurant Booking & Management System

## 📌 Project Overview

**Blu-Reserv** is a full-stack MERN-based restaurant booking and management system designed to handle table reservations, availability checks, notifications, and administrative access in a secure and scalable way.

This project was built as part of a team-based academic initiative, but throughout the development, it evolved into something much more than just a “college project.” It became a hands-on learning experience in **real-world software engineering**, **team collaboration**, **security awareness**, and **cloud-native deployment**.

---

## 🎯 Motivation & Vision

The core idea behind Blu-Reserv was simple:

> *Make restaurant bookings reliable, secure, and easy to manage.*

But as the project progressed, the scope naturally expanded to include:

* Multi-level authentication
* API exposure for third-party developers
* Cloud deployment
* Security testing and hardening
* CI/CD practices

This shift helped us understand how **real products evolve iteratively**, not all at once.

---

## 🧩 Key Features Implemented

### 🔹 Booking & Availability Management

* Create bookings with seat availability validation
* Prevent overbooking using business logic checks
* Centralized booking storage in MongoDB

### 🔹 Authentication & Access Control

* **Manager login** using credentials stored securely in the database
* **IBM SSO authentication** for enterprise-grade login
* **Demo user login** for easy testing and demonstrations
* Passwords stored using **hashed values**, never in plain text

### 🔹 API for Third-Party Developers

* REST APIs documented using **Swagger (OpenAPI)**
* Interactive API testing via Swagger UI
* Clear request/response schemas for external developers

### 🔹 Notifications

* Email notifications using SMTP (credentials stored securely via environment variables)
* SMS notification support using Twilio (test environment)

---

## 🛠️ Technology Stack

### Frontend

* React
* Modern component-based UI
* Environment-based configuration

### Backend

* Node.js & Express
* MongoDB
* RESTful API design
* Middleware-based architecture

### Deployment & Containerization

* **Podman** for containerization
* **Red Hat OpenShift** for deployment
* OpenShift Routes for external access
* Environment variables for configuration and secrets

---

## 🔁 Development Methodology

### Agile Development

* Followed an **iterative Agile approach**
* Features were built incrementally:

  1. Generic landing page
  2. Direct access to main page
  3. Manager login
  4. IBM SSO integration
  5. Demo user login
* Continuous testing and refinement based on feedback

This helped us understand that **software is built step-by-step**, not perfectly in the first attempt.

---

## 🔧 Version Control & Collaboration

* Git & GitHub for version control
* Feature-based branching strategy:

  * `main` → stable production-ready code
  * `feature/*` → isolated development
* Pull requests used to merge features
* Conflict resolution and code reviews strengthened team collaboration

---

## 🚀 CI/CD Pipeline

* Implemented **CI/CD using GitHub Actions**
* Automated steps include:

  * Dependency installation
  * Running unit tests
  * Security checks
* Helped catch issues early and ensured consistent builds

---

## 🧪 Testing Strategy

### Unit Testing

Focused on **core business logic**, especially booking integrity.

Covered test cases:

1. **Successful booking creation**
   Ensures the API returns `201 Created` for valid requests.

2. **Validation failure**
   Ensures the API returns `400 Bad Request` when required fields are missing.

3. **Business logic failure**
   Ensures the API returns `400 Bad Request` when requested seats exceed availability.

These tests helped prevent regressions and enforce correct system behavior.

---

## 🔐 Security Practices

### Dependency Security

* Used `npm audit` and `npm audit fix` to detect and resolve vulnerable packages

### Static & Dynamic Security Testing

* **SAST**: Static analysis using dependency and code-level scans
* **DAST**: Dynamic testing using **OWASP ZAP** on the running application

The DAST scan revealed:

* Low-risk configuration and informational alerts
* No critical vulnerabilities

This taught us that **security is often about configuration and awareness**, not just attacks.

### Secrets Management

* All sensitive credentials stored in `.env` files
* `.env` excluded from version control
* No secrets exposed to frontend or committed to GitHub

---

## 📚 What We Learned (Beyond Code)

### 💻 Technical Learnings

* How real backend APIs are designed and secured
* Importance of validation and business logic
* Practical use of cloud platforms like OpenShift
* Containerization concepts using Podman
* API documentation and developer experience

### 🧠 Managerial Learnings

* Importance of breaking work into small, manageable features
* Coordinating changes across frontend, backend, and deployment
* Handling merge conflicts and shared responsibilities
* Planning future improvements instead of overengineering early

### ❤️ Personal & Emotional Growth

* Learning to debug patiently instead of panicking
* Understanding that errors are part of development
* Gaining confidence in reading logs, security reports, and tool outputs
* Moving from “just writing code” to **thinking like an engineer**

---

## 🔮 Future Scope

* Role-based access control (RBAC)
* Session management using access and refresh tokens
* API key-based access for third-party developers
* Rate limiting and API versioning
* Advanced analytics and reporting dashboards
* Automated security scans integrated into CI/CD

---

## 🏁 Conclusion

Blu-Reserv was not just about building a booking system —
it was about learning **how real software systems are built, secured, deployed, and maintained**.

This project strengthened our understanding of:

* Full-stack development
* Cloud-native deployment
* Security best practices
* Team collaboration

Most importantly, it helped bridge the gap between **theory and real-world engineering**.

