# Ecommerce Store with Admin Panel (FastAPI + HTML/JS)

This is a full-stack ecommerce web application developed using **FastAPI** (backend) and **HTML + JavaScript** (frontend), with **PostgreSQL** as the database. It supports two roles: **User** and **Admin**. Admins can add products while users can browse, add to cart, and place orders.

---

## Features

### User
- Register/Login with email and password
- Browse available products
- Add products to cart
- View cart contents
- Place orders
- View order history

### Admin
- Register/Login as admin
- Access Admin Panel
- Add new products (name, price, description, quantity)

---

##  Tech Stack

| Layer      | Tech                       |
|------------|----------------------------|
| Backend    | FastAPI (Python)           |
| Frontend   | HTML + JavaScript          |
| Database   | PostgreSQL                 |
| ORM        | SQLAlchemy                 |
| Auth       | OAuth2 + JWT Tokens        |

---

##  Project Structure

ecommerce_api/
├── main.py # Main FastAPI app
├── models.py # Database models
├── schemas.py # Pydantic schemas
├── crud.py # Business logic
├── auth.py # JWT authentication
├── database.py # DB config
└── static/
├── index.html # Frontend HTML
└── script.js # JavaScript frontend logic


---

## 🔄 How to Run

1. Clone the repo and install dependencies:
    ```bash
    pip install fastapi uvicorn sqlalchemy psycopg2-binary python-jose passlib[bcrypt]
    ```

2. Set up PostgreSQL and update `DATABASE_URL` in `database.py`.

3. Run backend:
    ```bash
    uvicorn main:app --reload
    ```

4. Open `static/index.html` in browser or run it using Live Server.

---

## 📷 Screenshots

- ✅ Login/Register
- 👑 Admin Panel for adding products
- 🛒 Cart and Place Order
- 📦 View Orders

---

## ✅ Status

This project is fully working:
- User/admin registration
- JWT authentication
- Role-based admin features
- Product listing, cart, and order system

---

## 📌 Future Enhancements

- Product images
- Update products and orders
- Admin dashboard for managing users/orders
- Deploy using Docker

---

