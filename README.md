# 📚 Django Library App

A simple Library Management API built with **Django REST Framework** and **PostgreSQL**.  
This project allows you to create users and manage books via REST API and a small frontend demo.

---

## 🚀 Features
- User management (UUID-based)
- Book management (CRUD)
- REST API with Django REST Framework
- PostgreSQL as database
- Demo frontend (`Frontend/index.html`) to interact with API

---

## 🛠 Requirements
- Python 3.11+  
- PostgreSQL (running locally on port 5432)  
- Git  
- Virtualenv (recommended)  

---

## ⚙️ Installation Steps

### 1. Clone the repository
```bash
git clone https://github.com/sateyender/library_django_app.git
cd library_django_app
```

### 2. Create and activate virtual environment
```bash
python -m venv venv
venv\Scripts\activate   # Windows
# source venv/bin/activate  
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Setup environment variables
Create a `.env` file in the **project root** (same level as `manage.py`) with the following content:

```
SECRET_KEY=your_secret_key
DEBUG=True
DB_NAME=library_app
DB_USER=postgres
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
```

👉 For reference, you can use `.env.example` included in repo.

### 5. Run migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create superuser (admin)
```bash
python manage.py createsuperuser
```

### 7. Run development server
```bash
python manage.py runserver
```
App will be available at: **http://127.0.0.1:8000/**

---

## 📄 `.env.example`

```
SECRET_KEY=django-insecure-demo-key
DEBUG=True
DB_NAME=library_app
DB_USER=postgres
DB_PASSWORD=postgres
DB_HOST=localhost
DB_PORT=5432
```

 


---

## 📡 API Endpoints
- `GET /api/users/` → List users  
- `POST /api/users/` → Create user  
- `GET /api/books/` → List books  
- `POST /api/books/` → Create book  
- `PUT /api/books/{id}/` → Update book  
- `DELETE /api/books/{id}/` → Delete book  

---

##  Frontend Demo
A simple HTML file is included in `Frontend/index.html`.

Steps to use:
1. Start Django server (`python manage.py runserver`)
2. Open `Frontend/index.html` in browser
3. Use forms to create users and books, and view books list.

---

##  Author
**Sateyender Prajapati**  
📧 Email: sateyender1432@gmail.com  

---


