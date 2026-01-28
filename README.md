
# 🎫 HelpDesk Ticket Management System  
*A Full-Stack MERN Application*

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,nodejs,express,mongodb,jwt,git,github,vscode" />
</p>

---

## 📌 Project Overview

The **HelpDesk Ticket Management System** is a web-based application designed to manage user support requests (tickets) in an organized, secure, and efficient manner.

It allows **users** to raise issues and track their progress, while **admins/agents** can view, assign, prioritize, communicate, and resolve tickets systematically.

This project is built using the **MERN Stack** and follows real-world helpdesk workflows used in professional IT support systems.

---

## 🎯 MODULE 3: Ticket Management (Core Module)

This module represents the **heart of the application**.  
It controls the **complete lifecycle of a support ticket**, from creation to closure, including communication and tracking.

---

## 🔹 Functional Requirements

### 1️⃣ Ticket Creation & Lifecycle Management
- Users can raise support tickets with required details.
- Each ticket follows a defined lifecycle from **Open → Closed**.
- Ticket progress is continuously tracked.

### 2️⃣ Assignment & Prioritization
- Tickets can be assigned or reassigned to support agents (admins).
- Priority levels help agents decide which tickets need urgent attention.

### 3️⃣ Internal & External Communication
- Admins can communicate with users via replies.
- Internal notes are visible **only to admins**, not to users.

### 4️⃣ Ticket History & Audit Trail
- Every action on a ticket is recorded.
- Status changes and responses are preserved for transparency.

---

## ✨ Features (Exactly as Implemented)

### 🎟 Ticket Creation
Users can create a ticket by providing:
- **Subject**
- **Description**
- **Priority** (Low / Medium / High)

---

### 🔄 Ticket Status Management
Each ticket can have one of the following statuses:

- **Open** – Ticket is newly created
- **In Progress** – Ticket is being worked on
- **Waiting for Customer** – Awaiting user response
- **Resolved** – Issue fixed
- **Closed** – Ticket lifecycle completed

---

### 👤 Ticket Assignment
- Admins can **assign or reassign** tickets to agents.
- Ensures accountability and structured support handling.

---

### 💬 Communication System

#### Customer-Visible Replies
- Messages sent to users
- Used to request clarification or provide updates

#### Internal Notes
- Visible **only to admins**
- Used for internal discussion and troubleshooting

---

### 🕒 Ticket History & Tracking
- Maintains a complete log of:
  - Status updates
  - Replies
  - Internal notes
- Helps in audits and future reference

---

## 🔁 Overall Project Workflow (Non-Technical Explanation)

1️⃣ A **user logs in** and raises a support ticket  
2️⃣ The ticket is marked as **Open**  
3️⃣ An **admin views all tickets** from the dashboard  
4️⃣ Admin **assigns the ticket** and sets priority  
5️⃣ Admin communicates with the user if needed  
6️⃣ Ticket status changes based on progress  
7️⃣ Once resolved, the ticket is **closed**  
8️⃣ Full history is stored permanently  

This ensures **clear communication**, **traceability**, and **efficient issue resolution**.

---

## 🧠 Technical Workflow (Simple Terms)

- Frontend sends requests using **Axios**
- Backend handles logic via **Express controllers**
- Tickets stored in **MongoDB**
- Authentication secured using **JWT**
- Passwords hashed using **bcrypt**
- Role-based access (User / Admin)

---

## 🧱 Tech Stack

| Layer        | Technology |
|-------------|------------|
| Frontend    | React.js |
| Backend     | Node.js, Express.js |
| Database    | MongoDB |
| Authentication | JWT |
| Security    | bcrypt |
| Version Control | Git & GitHub |

---

## 📁 Project Folder Structure

```bash
HelpDesk-TicketManagement/
│
├── backend/
│   ├── config/
│   │   └── db.js
│   │
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── adminController.js
│   │   └── ticketsController.js
│   │
│   ├── middleware/
│   │   └── auth.js
│   │
│   ├── models/
│   │   ├── User.js
│   │   └── Tickets.js
│   │
│   ├── routes/
│   │   ├── auth.js
│   │   ├── admin.js
│   │   └── tickets.js
│   │
│   ├── scripts/
│   │   └── createAdmin.js
│   │
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── public/
│   │   └── index.html
│   │
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.js
│   │   │   └── PrivateRoute.js
│   │   │
│   │   ├── context/
│   │   │   └── AuthContext.js
│   │   │
│   │   ├── pages/
│   │   │   ├── Login.js
│   │   │   ├── Register.js
│   │   │   ├── Dashboard.js
│   │   │   ├── AdminDashboard.js
│   │   │   └── TicketDetail.js
│   │   │
│   │   ├── services/
│   │   │   └── api.js
│   │   │
│   │   ├── App.js
│   │   └── index.js
│   │
│   └── package.json
│
└── README.md
````

---

## 🔐 Security Highlights

* Passwords are **never stored in plain text**
* JWT ensures secure session handling
* Role-based access prevents unauthorized actions
* Internal notes are hidden from customers

---

## 🚀 Conclusion

The **Ticket Management (Module 3)** delivers a **real-world helpdesk experience**, combining usability, security, and structured workflows.
It demonstrates how modern web technologies can be used to build scalable support systems.

---

