# User Project Django Application

A Django project demonstrating user authentication and login functionality.

## Features

- User authentication system
- Login/logout functionality
- Template-based UI
- Admin interface

## Setup

1. **Navigate to project directory**
   ```bash
   cd userproject
   ```

2. **Install dependencies**
   ```bash
   pip install django
   ```

3. **Run migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create superuser**
   ```bash
   python manage.py createsuperuser
   ```

5. **Start development server**
   ```bash
   python manage.py runserver
   ```

6. **Access the application**
   - Main site: http://127.0.0.1:8000/
   - Admin panel: http://127.0.0.1:8000/admin/

## Project Structure

- `home/` - Main application with authentication views
- `templates/` - HTML templates for login and main pages
- `userproject/` - Project configuration