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
