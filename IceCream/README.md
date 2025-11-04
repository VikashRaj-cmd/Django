# Hello (Django demo)

This is a small Django demo project used for tutorial purposes.

Run (inside the `Hello` folder):

```powershell
python manage.py runserver
```

Notes:
- Database file `db.sqlite3` may exist in this folder. It's ignored by the root `.gitignore`.
- Do not commit real credentials or secrets to a public repository.
# Hello (Django project)

This is the `Hello` Django project. It contains a `home` app and templates under `templates/`.

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
- The project uses SQLite (`db.sqlite3`) located in this folder for local development.
- If templates or static files don't load, ensure `DEBUG = True` in `Hello/settings.py` during development.
