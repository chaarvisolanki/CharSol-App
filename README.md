# CharSol Forum App (Flask)
Minimal starter Flask forum app for Charvi Solanki's CharSol project.

## Features
- User registration & login (Flask-Login)
- Create & view posts (with optional image upload placeholder)
- Profile page
- SQLite database via SQLAlchemy
- Basic templates and styling

## Run locally
1. Create a virtualenv:
   python -m venv venv
   source venv/bin/activate   # on Windows: venv\Scripts\activate
2. Install dependencies:
   pip install -r requirements.txt
3. Initialize the database:
   flask --app app.py db init
   # (This project uses a simple create_db helper route on first run.)
4. Run:
   flask --app app.py run

## Notes
- This is a starter template. Extend models, add Supabase integration, OAuth, phone OTP, image storage (S3), and RLS later.
- For production use, configure SECRET_KEY environment variable and use a production-ready server.
