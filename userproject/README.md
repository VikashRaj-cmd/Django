# userproject (Django demo)

This project contains a simple login flow and templates for a demo site.

Local development admin credential (example only):

- username: `Admin`
- password: `Admin@123`

Please NOTE:
- These credentials are for local testing only. Do NOT push real credentials to GitHub or share them publicly.
- If you plan to publish this repository publicly, remove or change credentials and add instructions to create an admin account via `createsuperuser`.

How to verify or reset the admin password:

```powershell
cd "C:\Users\HP\Desktop\my code\Python Codewithharry\Django\userproject"
python manage.py shell

# In the Django shell:
from django.contrib.auth.models import User
User.objects.filter(username='Admin').values('username','is_superuser')
u = User.objects.get(username='Admin')
u.set_password('Admin@123')
u.save()
```

Or create a new superuser interactively:

```powershell
python manage.py createsuperuser
```
# userproject (Django project)

This is the `userproject` Django project. It contains a `home` app and templates under `templates/`.

Quickstart

1. Create and activate a Python virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies (if you have a `requirements.txt` in this folder):

```powershell
pip install -r requirements.txt
```

3. Apply migrations and start dev server:

```powershell
python manage.py migrate
python manage.py runserver
```

4. Visit http://127.0.0.1:8000/ to view the site.

Notes
- This project also uses SQLite (`db.sqlite3`) located in `userproject/` for local development.
