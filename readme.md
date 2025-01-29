# 🚀 Django Authentication System

A simple yet robust authentication system built with Django, featuring user login, logout, password change, and user management functionalities.

---

## ✨ Features
- 🔐 **User Authentication** using Django's built-in `LoginView` and `LogoutView`
- 🔄 **Secure Password Change** functionality
- 🎨 **Customizable Login Templates** for a better user experience
- 🎯 **Dashboard Redirection** after login
- 🚪 **Seamless Logout Redirection** to the login page
- 👥 **User Management:** Admins can **add, edit, delete, and view registered users**

---

## 🛠 Technologies Used
- 🐍 **Django** (Python-based web framework)
- 🎨 **HTML & CSS** (for frontend templates)
- 🗄 **SQLite** (default database, easily switchable to PostgreSQL/MySQL)

---

## ⚡ Installation Guide
### 1️⃣ Clone the Repository
```bash
    git clone https://github.com/AnushaGaneshan06/DjangoFullAuth-main.git
    cd DjangoFullAuth-main
```

### 2️⃣ Create a Virtual Environment
```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### 3️⃣ Install Dependencies
```bash
    pip install -r requirements.txt
```

### 4️⃣ Apply Migrations
```bash
    python manage.py migrate
```

### 5️⃣ Create a Superuser (Admin)
```bash
    python manage.py createsuperuser
```
Follow the prompts to set up an admin account.

### 6️⃣ Run the Server
```bash
    python manage.py runserver
```
Now, open `http://127.0.0.1:8000/` in your browser.

---

## 🔑 Usage Guide
### 🔹 Login
Navigate to `/login/` and enter your credentials.

### 🔹 Dashboard
Upon successful login, users are redirected to the **dashboard**.

### 🔹 Logout
Users can logout by visiting `/logout/`, which redirects them back to the login page.

### 🔹 Change Password
- Users can change their password at `/password_change/`.
- After a successful change, they are redirected to `/password_change/done/`.

### 🔹 User Management
Admins can:
- 👀 **View Registered Users:** Navigate to `/users/` to see all registered users.
- ✏️ **Edit Users:** Click on an individual user to modify details.
- 🗑 **Delete Users:** Remove users from the system.
- ➕ **Add New Users:** Register new users through the admin panel.

🔄 Refresh the Database
del db.sqlite3
python manage.py shell  
python manage.py migrate
python manage.py flush
python manage.py createsuperuser
python manage.py runserver
---

## 📂 Project Structure
```
project_root/
├── authentication_app/   # Django authentication app
│   ├── templates/
│   │   ├── registration/
│   │   │   ├── login.html
│   │   │   ├── password_change_form.html
│   │   │   ├── password_change_done.html
│   │   ├── dashboard.html
│   ├── views.py
│   ├── urls.py
│   ├── models.py
├── project_root/
│   ├── settings.py
│   ├── urls.py
├── manage.py
├── requirements.txt
└── README.md
```

---

## 🎨 Customization
- 🛠 Modify **`settings.py`** for custom authentication behavior.
- 🎨 Edit templates in **`templates/registration/`** for a personalized UI.
- 🔀 Update **`urls.py`** if you want different authentication routes.

---

## 🤝 Contributing
Pull requests are welcome! If you find issues or have suggestions, feel free to open an issue.

---

## Screenshots

<div style="display: flex; flex-wrap: wrap;">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/Register%20page.png" width="400" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/login%20page.png" width="400" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/Welcome%20profile%20page.png" width="500" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/all%20user%20info.png" width="500" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/Edit%20profile%20page.png" width="500" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/delete%20page.png" width="500" height="300">
  <img src="https://raw.githubusercontent.com/AnushaGaneshan06/DjangoFullAuth-main/89f45aab212ca7e26fcfee7f487ce3481d567d61/images/resent%20page.png" width="500" height="300">
</div>
## 🚀 Happy Coding! 🎉

