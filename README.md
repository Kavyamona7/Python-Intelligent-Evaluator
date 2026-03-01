Intelligent Evaluator

AI-Powered Python Code Evaluation Platform

A secure full-stack web application that automates Python programming assessment using semantic AI grading and static code analysis.

Built for academic environments to replace manual grading with scalable, intelligent evaluation.

🚀 What It Does

Professors create and publish coding challenges

Students submit Python solutions (paste or .py upload)

AI evaluates submissions using semantic analysis

Generates:

✅ Score

📝 Summary

💡 Constructive feedback

Advanced “Deep Evaluation” provides:

Code quality metrics

Maintainability index

Complexity analysis

Security linting

🏗 Tech Stack

Frontend

React + Vite + TypeScript

Tailwind CSS

Axios (JWT integration)

Backend

Flask (REST API)

SQLAlchemy ORM

Flask-JWT-Extended

bcrypt password hashing

Database

MySQL

AI & Analysis

LLM-based semantic grading

Streamlit microservice

Radon, Bandit, Flake8

🔐 Security

JWT-based authentication

Role-based access control (Professor / Student)

Hashed passwords (bcrypt)

ORM-protected database queries

Safe file handling

Sandboxed evaluation environment

📡 Core API
POST   /api/auth/login
GET    /api/challenges/?status=published
POST   /api/submissions/
POST   /api/deep-eval/launch
⚙️ Local Setup
Backend
cd backend
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python -m backend.main
Frontend
cd frontend
npm install
npm run dev
🧩 Key Design Highlights

Stateless REST architecture

Role-aware dashboards

Hybrid AI + optional runtime test evaluation

Auto-launching Deep Evaluation microservice

Extensible grading framework

👥 Roles

Professor

Create/manage challenges

View submissions

Monitor performance

Student

Submit code

View scores & feedback

Track history
