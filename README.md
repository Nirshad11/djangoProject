# MediCare Pharmacy Management System

A complete Django project for a Python OOP2 course project.

## One-click Windows setup

Double-click **setup.bat**. It creates `venv`, installs Django/Pillow, creates the SQLite database, inserts demo data, and starts the server.

If PowerShell is preferred, run `setup.ps1`.

## Manual commands

```bash
python -m venv venv
# Windows: venv\\Scripts\\activate
# macOS/Linux: source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py seed_demo
python manage.py runserver
```

Open http://127.0.0.1:8000/

Demo login: **admin** / **admin123**

## Features

- Login/logout with Django authentication
- Dashboard with inventory, suppliers, sales and revenue summary
- Medicine inventory CRUD, search, expiry and low-stock alerts
- Supplier management
- Sales entry with automatic stock deduction
- Invoice detail and print view
- Django admin at `/admin/`
