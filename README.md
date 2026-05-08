🎓 Student Achievements Tracker
A centralized digital platform to simplify and modernize the way student accomplishments are recorded and managed in academic institutions.

📌 Overview
The Student Achievements Tracker replaces traditional manual methods such as paper records and Excel sheets with a secure, web-based system. Students can upload certificates related to curricular and co-curricular activities, while faculty and HODs can review and approve them through a dedicated dashboard.

🚩 Problem Statement

Manual record-keeping using paper files or Excel sheets is time-consuming and error-prone
Verification process is inefficient and slow
High chances of mismanagement and data loss
Limited accessibility to past achievements
Lack of transparency in the approval process between students, faculty, and HODs


✅ Key Features

Web Application — Accessible anytime, anywhere for seamless record management
Role-Based Access — Secure logins for students, faculty, and HODs
Approval Dashboard — Centralized view for HODs to review and approve submissions
Efficient Workflow — Faster, transparent, and organized achievement tracking
Real-Time Notifications — Keeps users updated on approval status
Secure Data Storage — Certificates stored digitally to prevent loss or mismanagement


🛠️ Tech Stack
LayerTechnologyFrontendHTML, CSS, JavaScriptBackendPython (Flask)DatabaseSQLiteHostingWeb ServerNotificationsReal-time update system

👥 User Roles

Student — Upload certificates and track approval status
Staff/Faculty — Review and forward student submissions
HOD — Approve or reject achievements via dashboard


🚀 Getting Started
Prerequisites

Python 3.x
pip

Installation
bash# Clone the repository
git clone https://github.com/Abhisathwika05/Student-Achievements-Tracker.git
cd Student-Achievements-Tracker

# Create virtual environment
python -m venv venv
venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py
Then open your browser and go to http://localhost:5000

📂 Project Structure
StudentAchievementTracker/
├── templates/          # HTML templates
├── static/             # CSS, JS, images
├── models.py           # Database models
├── routes.py           # Application routes
├── auth.py             # Authentication logic
├── analytics.py        # Analytics module
├── main.py             # Application entry point
└── config.py           # Configuration settings

🔒 Security

Role-based access control for all user types
Secure file storage for uploaded certificates
Session-based authentication


📃 License
This project was developed as part of an academic initiative to digitize student achievement management.
