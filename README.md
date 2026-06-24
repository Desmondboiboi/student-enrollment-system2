# MMU Student Enrollment System (SES)

**TSE6223 Software Engineering Fundamentals — Trimester March/April 2026**
**Faculty of Information Science & Technology, Multimedia University**

A web-based Student Enrollment System built with **PHP**, **MySQL**, **HTML**, **CSS**, and a touch of **JavaScript**. The system implements the functional and non-functional requirements specified in the project report (FR-01 to FR-25, NFR-01 to NFR-08), and matches the many UI screens described in Section 6.3.

# System Installation and Setup Guide

To run the MMU Student Enrollment System (SES), please follow the steps below.

### Step 1: Install XAMPP

Download and install XAMPP from:

https://www.apachefriends.org/

After installation, open the XAMPP Control Panel.

### Step 2: Download the Project Files

Download the project ZIP file from the GitHub repository:

https://github.com/Desmondboiboi/student-enrollment-system2

Click **Code → Download ZIP**.

### Step 3: Extract the Project Folder

Extract the downloaded ZIP file into the XAMPP **htdocs** directory.

Example location:

```
C:\xampp\htdocs\
```

After extraction, the folder structure should be:

```
C:\xampp\htdocs\student-enrollment-system2\
```

### Step 4: Start Apache and MySQL

Open the XAMPP Control Panel and start:

* Apache
* MySQL

Ensure both services show the green "Running" status.

### Step 5: Open phpMyAdmin

Click the **Admin** button beside **MySQL**.

This will open phpMyAdmin in your web browser.

### Step 6: Create the Database

Navigate to:

```
student-enrollment-system2/mmu_ses/database/ses_setup.sql
```

Open the file using a text editor and copy all SQL statements.

In phpMyAdmin:

1. Click the **SQL** tab.
2. Paste the copied SQL script.
3. Click **Go / Execute**.

If successful, the system database and sample data will be created automatically.

### Step 7: Launch the System

Click the **Admin** button beside **Apache**, or open the following URL manually:

```
http://localhost/student-enrollment-system2/
```

Locate and open the **MMU Student Enrollment System**.

The login page will be displayed, indicating that the installation was successful.

```
http://localhost/mmu_ses/
```
You will be redirected to the login page.

---

## 🔑 Demo Credentials

Password for **all** demo accounts: `password123`

### Students (login as: Student)
| Student ID    | Name                          | Programme | Trimester |
|---------------|-------------------------------|-----------|-----------|
| `253UT256KY`  | Andrew Lim Zi Fei             | AI        | 2         |
| `253UT256JW`  | Desmond Choi Lip Sheng        | AI        | 2         |
| `243UT245X0`  | Siti Saimah Binti Abd Hamid   | AI        | 2         |
| `261UT240PM`  | Lim Yee Chen                  | AI        | 2         |

### Administrators (login as: Administrator)
| Admin ID  | Name                |
|-----------|---------------------|
| `ADM001`  | Dr. Tan Wei Ming    |
| `ADM002`  | Ms. Lim Su Yin      |

---

## 📁 Project Structure

```
mmu_ses/
│
├── README.md
├── index.php
├── login.php
├── register.php
├── logout.php
│
├── assets/
│   ├── css/
│   │   └── style.css
│   └── js/
│
├── config/
│   └── config.php
│
├── database/
│   ├── ses_setup.sql
│   └── ses_migration_v1_to_v2.sql
│
├── includes/
│   ├── auth.php
│   ├── bootstrap.php
│   ├── db.php
│   ├── db_credentials.php
│   ├── header.php
│   └── footer.php
│
├── controllers/
│   ├── AuthController.php
│   └── EnrollmentController.php
│
├── models/
│   ├── Database.php
│   ├── StudentModel.php
│   ├── CourseModel.php
│   ├── EnrollmentModel.php
│   ├── PrerequisiteModel.php
│   └── AdminModel.php
│
├── student/
│   ├── dashboard.php
│   ├── courses.php
│   ├── my_courses.php
│   ├── timetable.php
│   ├── profile.php
│   ├── slip.php
│   └── waitlist.php
│
└── admin/
    ├── dashboard.php
    ├── students.php
    ├── courses.php
    ├── enrollments.php
    ├── prerequisites.php
    └── reports.php
```

## 👥 Team

**Team Name:** The Tech Titan

| Student ID    | Name                          | Programme |
|---------------|-------------------------------|-----------|
| 253UT256KY    | Andrew Lim Zi Fei             | AI        |
| 253UT256JW    | Desmond Choi Lip Sheng        | AI        |
| 243UT245X0    | Siti Saimah Binti Abd Hamid   | AI        |
| 261UT240PM    | Lim Yee Chen                  | AI        |
