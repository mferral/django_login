# Django Email Login

## Overview

This project is a web application built using Django 5. It includes a basic setup with user authentication with email.

## Features

- User authentication (email login, registration)

## Requirements

- Python 3.8+
- Django 5.0
- SQLite (default) 

## Installation

1. **Clone the repository:**
   ```bash
   git clone `https://github.com/mferral/django_login.git`
   cd django_login
   ```
2. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3. **Apply the migrations:**
    ```bash
    python manage.py migrate
    ```
4. **Create a superuser:**
    ```bash
    python manage.py createsuperuser
    ```
5. **Run the development server:**
    ```bash
    python manage.py runserver
    ```
Open your web browser and navigate to http://127.0.0.1:8000.

## Usage
- Access the admin interface at `http://127.0.0.1:8000/admin` to manage users.
- Register a new user

## Test
1. **Open any HTTP Client:**
    URL: `http://127.0.0.1:8000/token/obtain`
    Method: **POST**
    Request:
    ```js
    {
        "email": "user@email.com",
        "password": "supersecret"
    } 
    ```
    Response:
    ```js
    {
	    "refresh": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTcyMjM2MjcxOCwiaWF0IjoxNzIyMjc2MzE4LCJqdGkiOiJjMGE2NzExZmM2MjY0NGVhODczZGIwMjQ4YzNhZWMyMCIsInVzZXJfaWQiOjIsImVtYWlsIjoibWZlcnJhbEBvdXRsb29rLmNvbSJ9.ZWV0BnBHnqaGKTWZuNQcaZh61HtBo56DEWYZQJgKT-Q",
	    "access": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNzIyMjc2NjE4LCJpYXQiOjE3MjIyNzYzMTgsImp0aSI6IjEwMDQ2MDUyYTBkYjQ4YmJiOTg4ZmUzN2UzMmRlNmI4IiwidXNlcl9pZCI6MiwiZW1haWwiOiJtZmVycmFsQG91dGxvb2suY29tIn0.l4V6AMfcwn8bIGcFzL4jaIdKmq-JjI_lUWoIZcMGIzA"
    }
    ```
    