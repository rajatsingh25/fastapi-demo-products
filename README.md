# FastAPI Product Management Application

A full-stack Product Management application built using **FastAPI** for the backend and **React** for the frontend.  
This project demonstrates clean API-first backend design, request validation, dependency injection, and frontend integration.

---

## 🚀 Tech Stack

### Backend
- **Python 3**
- **FastAPI**
- **SQLAlchemy**
- **Pydantic**
- **SQLite**
- **Uvicorn**

### Frontend
- **React**
- **JavaScript**
- **HTML / CSS**

---

## 📂 Project Structure

.
├── main.py # FastAPI application entry point
├── database.py # Database configuration and session management
├── database_models.py # SQLAlchemy ORM models
├── models.py # Pydantic schemas for request/response validation
├── requirements.txt # Backend dependencies
├── .gitignore
├── frontend/
│ ├── package.json
│ ├── public/
│ └── src/
│ ├── App.js
│ └── components


---

## 🧠 Key Features

- Automatic API documentation using **OpenAPI / Swagger**
- Request and response validation using **Pydantic**
- Dependency Injection for database session handling
- RESTful API design (API-first approach)
- Clean separation between:
  - Database models
  - API schemas
  - Application logic
- Frontend integration using React

---

## 🔄 Application Flow

Client (React UI)
↓
FastAPI Routes
↓
Pydantic Validation
↓
Dependency Injection (DB Session)
↓
SQLAlchemy ORM
↓
JSON Response


---

## ▶️ How to Run the Backend

### 1️⃣ Create Virtual Environment
```bash
python -m venv myenv
source myenv/bin/activate   # Linux / Mac
myenv\Scripts\activate      # Windows


2️⃣ Install Dependencies

pip install -r requirements.txt

3️⃣ Start FastAPI Server
uvicorn main:app --reload

4️⃣ Open API Docs

Swagger UI: http://127.0.0.1:8000/docs

ReDoc: http://127.0.0.1:8000/redoc

▶️ How to Run the Frontend

cd frontend
npm install
npm start
Frontend runs at:http://localhost:3000

| Method | Endpoint   | Description        |
| ------ | ---------- | ------------------ |
| GET    | /          | Health check       |
| GET    | /products/ | Fetch all products |


🔐 Security Notes

This is a demo project.
For production, the following should be added:

JWT authentication (OAuth2)

Role-based access control

Input sanitization

Rate limiting

🚀 Future Improvements

JWT Authentication

Async SQLAlchemy

Alembic migrations

Docker & Docker Compose

Redis caching

Unit & integration tests

Cloud deployment (AWS / GCP)

🧑‍💻 Author

Rajat Singh
Python Backend Engineer
FastAPI | REST APIs | SQLAlchemy
