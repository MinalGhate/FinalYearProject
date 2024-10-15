# Project Title : TLS/SSL Certificate analyser

## Description





## Installation

### Prerequisites

- Python 3.12 
- Django 3.x or later
- pip (Python package installer)

# Project Setup Instructions

## 1. Clone the Repository

```bash
git clone https://github.com/Priyanshi0912/FinalYearProject.git
```

## 2. Navigate to the Project Directory
```
cd wcd
```
## 3. Create and Activate a Virtual Environment
```
python -m venv virt
source virt/Scripts/activate   
```

## 4. Install the Required Dependencies
```
pip install django
pip install mysql
pip install mysql-connector-python
pip install -r requirements.txt
```
## 5. Apply Migrations to Set Up the Database
```
django-admin startproject wcd
python manage.py startapp website
```

## 6. Database setup
Add the following configuration to your `settings.py` file for the MySQL database:

```
DATABASES = {
    "default": {
        "ENGINE": "django.db.backends.mysql",
        "NAME": "elderco",
        "USER": "name_of_your_root_user",
        "PASSWORD": "your_mymysql_password",
        "HOST": "localhost",
        "PORT": "3306",
    }
}
```

```
touch mydb.py
```

## 7. Create a Superuser Account
```
python manage.py migrate
winpty python manage.py createsuperuser  
```
## 8. Run the Development Server
```
python manage.py runserver
```

## 9. Access the Application in Your Web Browser

http://127.0.0.1:8000



## Project Structure

Project Structure:
```
├── FinalYearProject/
│   ├── node_modules/
│   ├── virt/
│   │   ├── Include/
│   │   ├── Lib/
│   │   ├── Scripts/
│   │   └── pyvenv.cfg
│   ├── wcd/
│   │   ├── static/
│   │   │   ├── staticfiles/
│   │   │   │   ├── admin/
│   │   │   │   │   ├── css/
│   │   │   │   │   ├── img/
│   │   │   │   │   └── js/
│   │   ├── __pycache__/
│   │   ├── __init__.py
│   │   ├── asgi.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
├── website/
│   ├── __pycache__/
│   ├── migrations/
│   ├── templates/
│   │   ├── analyze.html
│   │   ├── analyzed_urls.html
│   │   ├── grading_system.html
│   │   ├── home.html
│   │   ├── login.html
│   │   ├── notification_alert.html
│   │   ├── recommendations.html
│   │   ├── register.html
│   │   └── send_email.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
├── mydb.py
├── package-lock.json
├── package.json
├── README.md
└── tailwind.config.js
```
