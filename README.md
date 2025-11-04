# Django Multi-Project Workspace

This repository contains two small Django projects used for learning and development:

- `Hello/` — demo project from the tutorial
- `userproject/` — another demo project with a login flow

WARNING: This workspace includes example credentials for local development only. Do NOT use these credentials in production or push real secrets to a public repository.

Admin credentials (local development example):

- username: `Admin`
- password: `Admin@123`

Quick start (Windows / PowerShell):

1. Open PowerShell and change to the project folder:

```powershell
cd "C:\Users\HP\Desktop\my code\Python Codewithharry\Django\userproject"
```

2. Create and activate a virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install Django if needed:

```powershell
pip install django
```

4. Run the development server:

```powershell
python manage.py runserver
```

5. Create a superuser (if you want to override the example credentials):

```powershell
python manage.py createsuperuser
```

See the per-project READMEs for more details.

## Push to GitHub

Two main options: use GitHub CLI (`gh`) or add a remote manually.

Using `gh` (recommended):

```powershell
# create a new repo on GitHub under your account and set it as origin
gh repo create <your-username>/<repo-name> --public --source=. --remote=origin --push
```

Manual remote add:

```powershell
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

Replace `<your-username>` and `<repo-name>` with your values.

## Admin account notes and verification

If you want to verify or reset the example admin account (`Admin` / `Admin@123`) run:

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

Or create a new superuser interactively (recommended):

```powershell
python manage.py createsuperuser
```

Security reminder: never commit real credentials into a repo. If you push this repository publicly, remove credential notes from the README or change the example credentials immediately.

# Django Multi-Project Workspace

This repository contains two Django projects used for learning and demos:

- `Hello/` - a Django project with templates and a simple `home` app.
- `userproject/` - another Django project (authentication demo and templates).

Each project is self-contained with its own `manage.py` and `settings.py`.

Getting started (per-project):

1. Create and activate a Python virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies (if you have a `requirements.txt` file in the project root or project folder):

```powershell
pip install -r requirements.txt
```

3. Run migrations and start the dev server for a chosen project (example for `Hello`):

```powershell
cd Hello
python manage.py migrate
python manage.py runserver
```

4. Open http://127.0.0.1:8000/ in your browser.

Notes
- This repository includes SQLite databases (`db.sqlite3`) for local development. Back them up before deleting.
- Add a `requirements.txt` to pin dependencies if you plan to share the project.

See the per-project README files for project-specific notes and usage.
