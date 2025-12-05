# Django Learning Projects

This repository contains two Django projects for learning and demonstration purposes:

- **IceCream/** - Django project with templates and a home app
- **userproject/** - Django project with authentication features

## Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Django
   ```

2. **Create virtual environment**
   ```bash
   python -m venv .venv
   # On Windows
   .venv\Scripts\activate
   # On macOS/Linux
   source .venv/bin/activate
   ```

3. **Install Django**
   ```bash
   pip install django
   ```

4. **Run a project** (example with IceCream)
   ```bash
   cd IceCream
   python manage.py migrate
   python manage.py runserver
   ```

5. **Create admin user**
   ```bash
   python manage.py createsuperuser
   ```

## Project Structure

Each project is self-contained with its own:
- `manage.py` - Django management script
- `settings.py` - Project configuration
- `templates/` - HTML templates
- `static/` - Static files (CSS, JS, images)

## Important Notes

- **Security**: Change the SECRET_KEY in settings.py before deploying
- **Database**: Projects use SQLite for development (db.sqlite3)
- **Debug Mode**: Set DEBUG=False in production

## Contributing

This is a learning repository. Feel free to fork and experiment!