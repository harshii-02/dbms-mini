
```markdown
# 🚆 Train Ticket Booking System 🎫

A mini-DBMS web project that simulates a train ticket booking system. This system allows users to log in, view available trains, and (for admins) manage train schedules via a simple interface connected to a MySQL backend.

---

## 🔧 Tech Stack

- **Python (Flask)** – Backend web framework  
- **MySQL** – Relational database  
- **HTML/CSS (Jinja2 templates)** – Frontend templating  

---

## 🚀 Features

- 🔐 Login System for Admins & Users
- 🛤️ View Available Trains
- ➕ Add New Trains (Admin)
- 📝 Update / Delete Train Details (Admin)
- 👥 Session Management with Flask



---

## 📁 Project Structure

```

dbms-mini/
├── app.py               # Main Flask app
├── templates/
│   ├── add.html         # Add train form
│   ├── admin.html       # Admin dashboard
│   ├── index.html       # Train list page
│   ├── login.html       # Login form
│   ├── update.html      # Update train form
│   └── user.html        # User dashboard
├── static/              # (optional) CSS/JS
└── README.md            # This file

````

---

## 🖥️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/harshii-02/dbms-mini.git
cd dbms-mini
````

### 2. Install Dependencies

```bash
pip install flask mysql-connector-python
```

### 3. Configure MySQL

Create a database named `appy` and run:

```sql
CREATE TABLE Admin (
  id INT AUTO_INCREMENT PRIMARY KEY,
  Username VARCHAR(50),
  Password VARCHAR(100)
);

CREATE TABLE User (
  id INT AUTO_INCREMENT PRIMARY KEY,
  Username VARCHAR(50),
  Password VARCHAR(100)
);

CREATE TABLE Train (
  id INT AUTO_INCREMENT PRIMARY KEY,
  Name VARCHAR(100),
  Cost DECIMAL(10, 2),
  Distance DECIMAL(10, 2),
  Date DATE
);
```

Insert a test admin:

```sql
INSERT INTO Admin (Username, Password) VALUES ('admin', 'admin123');
```

### 4. Run the Application

```bash
python app.py
```

Visit `http://127.0.0.1:5000` in your browser.

---

## 📘 Notes

* This project was developed as part of a **Database Management System (DBMS) mini-project**.
* Educational/demo use only.

---

## 🪪 License

Licensed under the **MIT License**.

---

## 🙋‍♀️ Author

**Harshii**
🔗 [GitHub Profile](https://github.com/harshii-02)

```



