# Django Authentication (Login & Logout) with Templates

## Overview
This project demonstrates user authentication in **Django**, including **login and logout**, using Django's built-in authentication system with **HTML templates** for rendering pages.

## Features
- User **Registration**
- User **Login & Logout**
- Django's **built-in authentication** system
- **Session-based authentication**
- **Bootstrap-based templates** for UI

## Tech Stack
- **Backend**: Django
- **Frontend**: HTML, CSS (Bootstrap)
- **Database**: SQLite (default) / PostgreSQL (optional)

---

## Installation & Setup

### 1. Clone the Repository
```sh
git clone https://github.com/BVSK203/authontication-login-logout.git
cd authontication-login-logout
```

### 2. Setup Virtual Environment
```sh
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```sh
pip install -r requirements.txt
```

### 4. Apply Migrations
```sh
python manage.py migrate
```

### 5. Create a Superuser (Optional)
```sh
python manage.py createsuperuser
```

### 6. Run the Server
```sh
python manage.py runserver
```
Access the app at: `http://127.0.0.1:8000/`

---

## URL Routes
| Route | Description |
|-------|------------|
| `/register/` | User Registration |
| `/login/` | User Login |
| `/logout/` | User Logout |
| `/dashboard/` | Protected Dashboard Page |

---

## Project Structure
```
project_root/
│── authentication_app/
│   ├── templates/
│   │   ├── login.html
│   │   ├── register.html
│   │   ├── dashboard.html
│   │   ├── base.html
│   ├── views.py
│   ├── urls.py
│   ├── models.py
│── static/
│── manage.py
```

---

## Authentication Flow
1. User **registers** using `/register/`.
2. User logs in using `/login/`.
3. Django creates a session and redirects to `/dashboard/`.
4. User logs out via `/logout/` and is redirected to the login page.

---

## Contribution
Feel free to fork this project and submit pull requests!

---

## License
MIT License. Free to use and modify.

