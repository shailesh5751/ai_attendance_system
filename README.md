# 🧠 AI-Assisted Attendance System 🎓

An AI-powered digital attendance system that leverages facial recognition technology to streamline and automate student attendance processes in educational institutions. This system is designed using modern deep learning tools and frameworks like **TensorFlow**, **OpenCV**, and **Django**, providing a robust and secure solution for real-time attendance management.

---

## 🚀 Features

- 🔍 **Face Recognition-Based Attendance**
  - Detects and identifies student faces using deep learning models.
- 🧾 **Automated Attendance Marking**
  - Automatically records attendance in a MySQL database once a face is recognized.
- 📋 **Admin Dashboard**
  - Django-based web interface for managing students, viewing reports, and exporting data.
- 🧠 **AI Model Integration**
  - Uses face encoding and matching logic with `face_recognition` library.
- 📸 **Live Camera Feed**
  - Real-time face detection using webcam or uploaded image.
- 📤 **Export Attendance Records**
  - Export reports in CSV/Excel formats.
- 🔐 **JWT Authentication**
  - Secure login and API protection using `djangorestframework-simplejwt`.

---

## 🛠️ Tech Stack

**Frontend:**
- React (future support)
- HTML/CSS (basic interface)

**Backend:**
- Django REST Framework
- Python
- OpenCV
- face_recognition
- JWT authentication

**Database:**
- MySQL

---

## ⚙️ Setup Instructions

### 🔧 Prerequisites

- Python 3.9+
- pip
- MySQL Server
- virtualenv (optional but recommended)

### 💻 Clone the Repository

```bash
git clone https://github.com/shailesh5751/ai_attendance_system.git
cd ai_attendance_system
```

### 📦 Install Dependencies
```bash
pip install -r requirements.txt
```
### 🔧 Configure Database

1. Create a MySQL database
2. Update settings.py in Django project:

```python
DATABASES = {
  'default': {
    'ENGINE': 'django.db.backends.mysql',
    'NAME': 'attendance_db',
    'USER': 'your_username',
    'PASSWORD': 'your_password',
    'HOST': 'localhost',
    'PORT': '3306',
  }
}
```
3. Apply Migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 🔐 Setup Superuser (Admin)
```bash
python manage.py createsuperuser
```

### ▶️ Run the Server
```bash
python manage.py runserver
```
Visit http://127.0.0.1:8000/admin/ to access the Django admin panel.

### 📁 Project Structure
```bash
ai_attendance_system/
├── attendance/              # Core app for attendance logic
├── users/                   # User authentication
├── encodings/               # Facial encoding logic
├── media/                   # Uploaded images / faces
├── templates/               # HTML templates (for admin UI)
├── static/                  # Static files
├── manage.py
└── requirements.txt
```

## 🔍 Future Enhancements
✅ React-based frontend with full UI support
✅ Email OTP verification for registration
✅ Role-based access control (admin, student)
📲 Mobile app integration
📈 Attendance analytics dashboard


## 🙋‍♂️ Maintainer
Shailesh More
📧 shailesh5751@gmail.com
🌐 LinkedIn
