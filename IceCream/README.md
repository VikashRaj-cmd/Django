# IceCream Django Project

A Django web application for an ice cream shop featuring multiple pages, contact forms, and responsive design.

## Features

- **Multi-page website** with navigation
- **Contact form** with database storage
- **Bootstrap responsive design**
- **Template inheritance** using base.html
- **Static file handling** for images
- **Admin interface** for managing contacts

## Setup

1. **Navigate to project directory**
   ```bash
   cd IceCream
   ```

2. **Install dependencies**
   ```bash
   pip install django
   ```

3. **Run migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

5. **Start development server**
   ```bash
   python manage.py runserver
   ```

6. **Visit the application**
   - Main site: http://127.0.0.1:8000/
   - Admin panel: http://127.0.0.1:8000/admin/

## Project Structure

- `home/` - Main application with views, models, and URLs
- `templates/` - HTML templates (base.html, index.html, about.html, services.html, contact.html)
- `static/img/` - Static images
- `IceCream/` - Project configuration and settings

## Pages

- **Home** (`/`) - Welcome page with ice cream showcase
- **About** (`/about`) - Information about the ice cream shop
- **Services** (`/services`) - Available ice cream products and services
- **Contact** (`/contact`) - Contact form for customer inquiries

## Models

- **Contact** - Stores customer contact form submissions with fields for name, email, phone, and description