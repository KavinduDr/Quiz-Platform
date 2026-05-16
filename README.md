# Classroom Assessment & Student Quiz System

A comprehensive, full-stack examination and quiz management platform designed for educational institutions. The system features a decoupled, multi-repository architecture consisting of a robust TypeScript/Express backend, an interactive Student/Candidate Frontend, and a dedicated Instructor/Admin Management Dashboard.

---

## 🏗️ Architecture & Repositories

To ensure a clean separation of concerns, optimized deployment pipelines, and maximum scalability, the project is split into three dedicated repositories:

| Component | Responsibility | Tech Stack | Repository Link |
| :--- | :--- | :--- | :--- |
| **Backend API** | Centralized business logic, JWT authentication, database schemas, and Redis session caching. | Node.js, Express, TypeScript, Redis, Docker | [🔗 Backend Repo](https://github.com/neroIJN/classroom-assessment-system-backend) |
| **Student Frontend** | Portal for students to view dashboards, track active assignments, submit tests, and take live quizzes. | Next.js (App Router), React, Tailwind CSS | [🔗 Student Portal Repo](https://github.com/KavinduDr/Student-Dashboard) |
| **Lecturer Dashboard** | Administrative console for instructors to create/edit quizzes, grade essay-type answers, and analyze student metrics. | Next.js (App Router), Radix UI, Tailwind CSS | [🔗 Lecturer Dashboard Repo](https://github.com/KavinduDr/Lecturer-Dashboard) |

---

## 🚀 Key Features

### 🔹 Core System & Security
*   **Secure Authentication:** State-driven JWT-based authentication system complete with sign-up, password reset, and activation flows.
*   **Session Management:** Fast data fetching and session handling assisted by a Redis caching layer.
*   **Containerized Architecture:** Backend application fully Dockerized for effortless cloud deployment.

### 🔹 Instructor Capabilities
*   **Dynamic Assessment Builder:** Dedicated interfaces for generating standard multiple-choice quizzes and elaborate essay-type evaluations.
*   **Granular Performance Analytics:** Dual-perspective reporting views structured both **per-quiz** (to track class averages) and **per-student** (to track individual growth).
*   **Evaluation Engine:** Custom workflows built to streamline review and grading of essay submissions.

### 🔹 Student Capabilities
*   **Intuitive Examination Interface:** Clean, focused layout designed for distraction-free quiz taking and assignment submissions.
*   **Live Violation Monitoring:** Context-driven UI state setup to ensure assessment integrity during evaluations.

---

## 🛠️ System-Wide Technical Stack

*   **Runtime Environment:** Node.js (v18+)
*   **Programming Language:** TypeScript, JavaScript
*   **Backend Framework:** Express.js
*   **Frontend Ecosystem:** Next.js (App Router), React 18, React Context API
*   **Styling & UI Primitives:** Tailwind CSS, Radix UI, NextUI
*   **Database & Caching:** Redis (Auxiliary/Session data), SQL/NoSQL (via Database Connection string)
*   **DevOps & Tooling:** Docker, npm / pnpm / yarn

---

## 💻 Local Setup & Development

To run the entire ecosystem locally, you will need to clone and configure each repository individually. 

### 1. Backend Setup
```bash
git clone [https://github.com/neroIJN/classroom-assessment-system-backend.git](https://github.com/neroIJN/classroom-assessment-system-backend.git)
cd classroom-assessment-system-backend
npm install
