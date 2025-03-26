# Django-gas-utility-system

A customer service portal for gas utilities with request tracking, user management, and admin dashboard.

## **🚀 Features**
- User registration & authentication (JWT tokens)
- Service request submission & tracking
- Admin dashboard for staff
- PostgreSQL database support
- Deployable to Render/Heroku

## **🛠️ Tech Stack**
- **Backend**: Django 4.2 + Django REST Framework
- **Database**: PostgreSQL
- **Auth**: JWT + Token Authentication
- **Deployment**: Render.com

## **⚙️ Setup**

### **1. Local Development**
```bash
# Clone repo
git clone https://github.com/your-username/gas-utility-system.git
cd gas-utility-system

# Set up virtual env (Windows)
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env
# Edit .env with your values

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Run server
python manage.py runserver



Django Application Code-Base Structure
gas-utility-system/
├── .env.example
├── .gitignore
├── requirements.txt
├── manage.py
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── apps/
    ├── accounts/
    │   ├── migrations/
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py          
    │   ├── models.py
    │   ├── serializers.py
    │   ├── urls.py          # All account URLs here
    │   └── views.py         
    │
    └── services/
        ├── migrations/
        ├── __init__.py
        ├── admin.py
        ├── apps.py          
        ├── models.py
        ├── serializers.py
        ├── urls.py          # All service URLs here
        └── views.py         
