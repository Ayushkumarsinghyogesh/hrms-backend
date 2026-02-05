## 🚀 Run Backend Locally (Django)

### Prerequisites
- Python 3.10 or 3.11
- pip
- virtualenv
- Git

---

### 1. Clone Repository
```bash
git clone https://github.com/Ayushkumarsinghyogesh/hrms-backend.git
cd hrms-backend


python3 -m venv venv
source venv/bin/activate   # Linux / macOS
# venv\Scripts\activate    # Windows

pip install --upgrade pip
pip install -r hrms/requirements.txt


cd hrms
python manage.py migrate


python manage.py runserver


Run with Gunicorn (Optional)
gunicorn hrms.wsgi:application --chdir hrms
