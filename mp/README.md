# Student Achievement Tracker (SAT)

## Overview
Student Achievement Tracker (SAT) is a web application designed to help educational institutions manage and track student achievements efficiently. The system allows students to upload certificates for various achievements, which are then reviewed and approved by staff and Heads of Departments (HODs). The platform also provides analytics and notifications to keep all users informed.

## Features
- User roles: Student, Staff (Class Teacher), Head of Department (HOD)
- Secure user authentication and role-based access control
- Students can upload achievement certificates with details
- Staff can review and approve/reject certificates submitted by their students
- HODs can perform final approval and view analytics for their department
- Notifications system for updates on certificate status
- Dashboard views tailored for each user role
- Analytics for student performance and achievements
- File upload support with optional AWS S3 cloud storage integration

## Technology Stack
- Python 3
- Flask web framework
- Flask-Login for authentication
- Flask-SQLAlchemy for ORM and database management
- SQLite  or other databases via SQLALCHEMY_DATABASE_URI
- AWS S3 for optional cloud storage of certificates
- HTML, CSS, JavaScript for frontend templates and static assets

## Installation and Setup

### Prerequisites
- Python 3.7 or higher
- pip package manager



### Create and activate a virtual environment
```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On Unix or MacOS
source venv/bin/activate
```

### Install dependencies
```bash
pip install -r requirements.txt
```



### Database Initialization
The app uses Flask-Migrate for database migrations.

To initialize the database and apply migrations:
```bash
flask db init
flask db migrate
flask db upgrade
```

Alternatively, the app creates tables automatically on startup if they don't exist.

### Running the Application
Run the Flask app with:
```bash
python app.py
```
The app will be available at `http://localhost:5000`.

## Usage

### Student
- Register and login
- Upload achievement certificates (PDF or JPEG)
- View dashboard with certificate stats and notifications
- View and download certificates
- Access analytics related to their achievements

### Staff (Class Teacher)
- Login to access dashboard
- View students assigned to them
- Review and approve/reject certificates uploaded by students
- Send feedback on certificates
- Receive notifications about certificate uploads and approvals

### Head of Department (HOD)
- Login to access dashboard
- View pending certificates approved by staff for final approval
- Approve or reject certificates with feedback
- View department-wide analytics and reports
- Manage notifications

## File Uploads and Storage
- Supports uploading PDF and JPEG files as certificates
- Files are stored locally in the `storage/` directory by default
- Optionally, files can be stored in AWS S3 if configured

## Project Structure
- `app.py`: Application entry point
- `__init__.py`: Flask app factory and setup
- `config.py`: Configuration settings
- `models.py`: Database models
- `routes.py`: Application routes and views
- `auth.py`: Authentication and role decorators
- `utils.py`: Utility functions
- `analytics.py`: Analytics functions
- `templates/`: HTML templates for different user roles
- `static/`: Static assets (CSS, JS)
- `storage/`: Uploaded certificate files
- `migrations/`: Database migration scripts


