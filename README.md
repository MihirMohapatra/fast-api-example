# 🚀 FastAPI Crash Course

A beginner-friendly FastAPI project demonstrating CRUD operations using an in-memory list. This project is ideal for learning the fundamentals of FastAPI, Pydantic models, and REST APIs.

---

## 📌 Features

- FastAPI framework
- RESTful API
- CRUD Operations
- Pydantic Models
- Interactive Swagger UI
- Automatic API Documentation

---

## 📁 Project Structure

```text
Fast-API-Crash/
│
├── venv/                  # Virtual Environment
├── main.py                # FastAPI Application
├── requirements.txt       # Project Dependencies
└── README.md              # Project Documentation
```

---

## 🛠️ Prerequisites

- Python 3.10+
- pip

Verify installation:

```bash
python --version
pip --version
```

---

## ⚙️ Create Virtual Environment

### Windows (PowerShell)

```powershell
python -m venv venv
.\venv\Scripts\Activate
```

### macOS/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 📦 Install Dependencies

```bash
pip install fastapi uvicorn
```

Or install all recommended packages:

```bash
pip install "fastapi[standard]"
```

---

## ▶️ Run the Application

```bash
python -m uvicorn main:app --reload
```

Expected output:

```text
INFO:     Uvicorn running on http://127.0.0.1:8000
```

---

## 🌐 API URLs

| Resource | URL |
|----------|-----|
| Home | http://127.0.0.1:8000 |
| Swagger UI | http://127.0.0.1:8000/docs |
| ReDoc | http://127.0.0.1:8000/redoc |

---

# 📚 API Endpoints

## Home

### GET /

Returns a welcome message.

Response

```json
{
  "message": "Welcome to chai code"
}
```

---

## Get All Teas

### GET /teas

Response

```json
[]
```

---

## Add Tea

### POST /teas

Request

```json
{
  "id": 1,
  "name": "Assam Tea",
  "origin": "India"
}
```

Response

```json
{
  "id": 1,
  "name": "Assam Tea",
  "origin": "India"
}
```

---

## Update Tea

### PUT /teas/{tea_id}

Request

```json
{
  "id": 1,
  "name": "Darjeeling Tea",
  "origin": "India"
}
```

---

## Delete Tea

### DELETE /teas/{tea_id}

---

## 📋 Tea Model

```python
class Tea(BaseModel):
    id: int
    name: str
    origin: str
```

---

## 📦 Generate Requirements

```bash
pip freeze > requirements.txt
```

Install later:

```bash
pip install -r requirements.txt
```

---

## 🧪 Testing

Open Swagger UI:

```
http://127.0.0.1:8000/docs
```

Use **Try it out** to test every endpoint.

---

## 🚀 Technologies Used

- Python
- FastAPI
- Uvicorn
- Pydantic

---

## 📖 Learning Objectives

- Build REST APIs with FastAPI
- Understand HTTP methods (GET, POST, PUT, DELETE)
- Learn request validation using Pydantic
- Explore interactive API documentation
- Work with path parameters and request bodies

---

## 🔮 Future Improvements

- SQLite/PostgreSQL Database
- SQLAlchemy ORM
- JWT Authentication
- Dependency Injection
- Docker Support
- Alembic Migrations
- Unit Testing
- Logging
- Environment Variables
- Project Modularization

---

## 👨‍💻 Author

**Mihir Kumar Mohapatra**

Senior Software Engineer

Learning FastAPI to build scalable, production-ready backend services.

---

##Ref: (Chai aur Code) https://www.youtube.com/watch?v=foGklduxhM0&pp=ygUHZmFzdGFwaQ%3D%3D
---

## ⭐ License

This project is for educational purposes.
