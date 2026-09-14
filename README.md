# Social Media API

## About
This project is a social media backend built with Django and Django REST Framework. It provides the core functionality for a social networking platform, including user accounts, profiles, posts, comments, likes, follows, and notifications.

The application is organized into reusable Django apps and is designed to serve as a solid foundation for building a full social media service API.

## Features
- Custom user authentication using a `User` model
- Profile management
- Post creation and updates
- Comments on posts
- Likes and follow relationships
- Notification support
- SQLite database for local development

## Tech Stack
- Python
- Django 6.1.1
- Django REST Framework 3.18.1
- Simple JWT for authentication

## Project Structure
- `config/` - Django project settings and URL configuration
- `users/` - user and profile models
- `socials/` - social app models such as posts, comments, likes, follows, and notifications
- `manage.py` - Django management entry point
- `requirements.txt` - Python dependencies
- `db.sqlite3` - local SQLite database

## Getting Started

### 1. Clone the repository
```bash
git clone <your-repository-url>
cd social_media_api
```

### 2. Create and activate a virtual environment
```bash
python -m venv .venv
```

On Windows PowerShell:
```powershell
.\.venv\Scripts\Activate.ps1
```

On macOS/Linux:
```bash
source .venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run database migrations
```bash
python manage.py migrate
```

### 5. Start the development server
```bash
python manage.py runserver
```

## Useful Commands
```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
python manage.py test
```

## GitHub Push Ready
This repository is set up to avoid committing local development artifacts such as:
- virtual environments
- Python cache files
- database files
- environment files
- editor and OS-generated files

Before pushing to GitHub, run:
```bash
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-github-repository-url>
git push -u origin main
```

## Notes
- The project currently uses SQLite for development.
- Sensitive values such as the Django secret key should be moved to environment variables or a local settings file in production.
- The `.gitignore` file is configured to keep local environment files and generated artifacts out of version control.
