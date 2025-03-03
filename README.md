# smartteck
private repo for smartteck log

#Smart KPI & Task Management System

📁 Project Documentation

# 🚀 KPI Dashboard with Role-Based Access Control

A **FastAPI + Streamlit** project that provides a **KPI Dashboard** with **role-based permissions** and **task management**.

## Features
✅ Superadmin, Admin, User roles  
✅ Role-based permissions (view/manage dashboards, assign tasks)  
✅ JWT-based authentication  
✅ Task assignment system  
✅ SQLite database integration  

---

## 🛠 Tech Stack
- **Backend:** FastAPI, SQLite, SQLAlchemy, JWT
- **Frontend:** Streamlit (for the KPI dashboard)
- **Authentication:** OAuth2 + JWT

---

## 📦 Installation

### 1️⃣ Clone the Repository
sh
git clone https://github.com/your-username/kpi-dashboard.git
cd kpi-dashboard


📁 Project Structure
bash
Copy
Edit
kpi-dashboard/
│── backend/
│   ├── main.py           # FastAPI server (Runs the backend)
│   ├── auth.py           # User authentication (JWT-based login)
│   ├── permissions.py    # Role-based permission system
│   ├── tasks.py          # Task assignment & management
│   ├── database.py       # SQLite Database configuration
│   ├── models.py         # Database models (SQLAlchemy)
│   ├── users.py          # User management (add/remove users)
│
│── frontend/
│   ├── app.py            # Streamlit UI (Main dashboard)
│   ├── pages/
│   │   ├── dashboard.py  # KPI Dashboard
│   │   ├── manage_users.py  # User & Group Management
│   │   ├── tasks.py      # Task Management
│
│── .env                  # Environment variables
│── requirements.txt      # Python dependencies
│── README.md             # Project Documentation


![kpi-dashboard_ - visual selection](https://github.com/user-attachments/assets/bd07231c-bd54-4e55-9952-adbb59446e12)


🛠 Frameworks & Tools Used
Technology	Purpose	Why Used?
FastAPI	- Backend API	- Fast, asynchronous, lightweight, built-in validation
Streamlit	- Frontend (Dashboard UI)	- Easy-to-use, Python-based, great for data apps
SQLite	- Database	- Lightweight, file-based, no setup needed
SQLAlchemy	- ORM (Database management)	- Allows Python-based database interactions
JWT (PyJWT)	- Authentication (User Login)	- Secure, token-based authentication
OAuth2	- Secure user authentication	- Industry-standard for auth, integrated with JWT
Requests	- API Calls (Frontend ↔ Backend) -	Allows frontend to communicate with backend
Uvicorn	- ASGI Server (Runs FastAPI) -	Fast, production-ready web server


📌 Why These Choices?

1️⃣ FastAPI (Backend)
Chosen because it's asynchronous, fast, and lightweight.
Comes with built-in data validation using Pydantic.
Supports JWT authentication out-of-the-box.
Works seamlessly with SQLAlchemy and OAuth2.

2️⃣ Streamlit (Frontend)
Super easy to use—just write Python, and it renders UI elements.
Built for data-driven applications (perfect for KPIs & dashboards).
No need for HTML, CSS, or JavaScript.
Provides tabs, buttons, and input fields out-of-the-box.

3️⃣ SQLite (Database)
No need for complex setup—just a single file (database.db).
Works perfectly with SQLAlchemy ORM.
Ideal for small to medium-scale applications.

4️⃣ SQLAlchemy (ORM)
Avoids writing raw SQL queries—just use Python classes.
Ensures database consistency and structure.
Works across different database engines (can be upgraded to PostgreSQL, MySQL).

5️⃣ JWT (JSON Web Tokens)
Stateless authentication (no need for session storage).
More secure than cookies—tokens are encrypted.
Allows user roles and permissions to be embedded in the token.

6️⃣ OAuth2 (Authentication)
Industry-standard authentication protocol.
Secure user login with token-based authentication.
Integrates easily with JWT for role-based permissions.

7️⃣ Requests (API Communication)
Allows Streamlit frontend to talk to the FastAPI backend.
Used for sending login requests, fetching data, and assigning tasks.

8️⃣ Uvicorn (ASGI Server)
FastAPI requires an ASGI server—Uvicorn is the best choice.
Highly optimized for handling multiple requests.
Used in production for deploying FastAPI applications.
