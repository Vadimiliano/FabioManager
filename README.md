# DiplomFabioManager
# Fabiomanager

A web application for warehouse accounting and order management, built for a real
client — **FABIOBRUNO LLC**. Developed as my diploma project.

## Screenshots
Screenshots of the main screens are available in the [screenshots](screenshots/) folder.

🎥 **Demo video:** https://vadimiliano.github.io

## Features

- **Materials accounting** — track materials in stock: incoming, outgoing and current balances
- **Customer orders** — create orders, update their status and track progress
- **Daily tasks for employees** — assign tasks to staff members
- **Role-based access** — three roles (Admin, Manager, Employee), each with its own permissions; secured with JWT authentication
- **Dashboards & charts** — visual overview of orders and key metrics

### Roles

| Role     | Can do                                                        |
|----------|---------------------------------------------------------------|
| Admin    | Manage users and roles, full access to all data               |
| Manager  | Create and manage orders, assign daily tasks, view dashboards |
| Employee | View and complete assigned tasks                              |

## Tech stack

| Part      | Technologies       |
|-----------|--------------------|
| Frontend  | React, TypeScript  |
| Backend   | Python, FastAPI    |
| Database  | PostgreSQL         |
| Auth      | JWT                |

## Getting started

### Requirements
- Node.js and npm
- Python 3.10+
- PostgreSQL

### Backend
```bash
cd backend
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

Create a PostgreSQL database and set the connection string in the backend config
before the first run.
