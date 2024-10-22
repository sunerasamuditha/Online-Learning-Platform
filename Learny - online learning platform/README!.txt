
===============================================================
# LEARNY - Online Learning Platform
===============================================================

LEARNY is an online learning platform developed by **Group 4** of the Web Development course. It provides an intuitive, user-friendly experience for both students and instructors, offering features like course creation, course navigation, and progress tracking.

---

## Installation Guide

### 1. XAMPP Setup

1. Download and install **XAMPP** from [here](https://www.apachefriends.org/index.html).
2. Copy the **LEARNY** project folder to the following directory:
   ```
   C:\xampp\htdocs\LEARNY
   ```

### 2. Database Setup

LEARNY uses two databases:
- `learnydb` - For managing user-related data (students/instructors).
- `course_management` - For managing course-related content (videos, documents, assignments).

#### Steps to set up the databases:
1. Open **phpMyAdmin** at `http://localhost/phpmyadmin/`.
2. Create two databases: 
   - `learnydb`
   - `course_management`
3. Import the SQL dump files found in the `database` folder:
   - `learnydb.sql`
   - `course_management.sql`
4. Check that the `config/database.php` file points to the correct databases:
   ```php
   'dbname' => 'learnydb' (for user data)
   'dbname' => 'course_management' (for course data)
   ```

---

## Folder Structure

### Backend (MVC Architecture)

LEARNY is built using a **Model-View-Controller (MVC)** architecture for efficient organization and scalability. The backend structure includes:

- **config/**: Contains database configurations and application settings.
- **controllers/**: Handles business logic and interactions with the models.
- **models/**: Manages database queries and handles data retrieval/manipulation.
- **views/**: Contains the HTML and templates used for user interface rendering.
- **functions/**: Reusable helper functions for common tasks.
- **public/**: Public folder with the main entry point (`index.php`).

### Frontend (Bootstrap Framework)

The frontend of LEARNY uses **Bootstrap** for responsive, user-friendly design. The structure of frontend files is as follows:

- **assets/**: Contains CSS, JavaScript, images, and other resources.
- **courses/**: Houses the courses listing page.
- **course details/**: Displays the details and content of each course.
- **dashboard/**: User dashboard for managing course progress and activities.
- **loginnew/**: Login page for both students and instructors.
- **registernew/**: Registration page for new users.
- **vendor/**: Third-party libraries and plugins used in the frontend.

---

## Key Features

1. **Single Page Home**: A smooth, intuitive landing page.
2. **User Role Management**: Separate login and registration for instructors and students.
3. **Course Management**: Instructors can create, upload, and manage course content (videos, assignments, documents).
4. **Course Navigation**: Students can navigate through courses, view videos, and download documents.
5. **Progress Tracking**: Students can track their learning progress with ease.

---

## Acknowledgments

Special thanks to:
- Our instructors for their guidance throughout the project.
- Our classmates for their feedback and suggestions.
- The open-source community whose tools and libraries were instrumental in developing LEARNY.

---

## Copyright

© 2024 **LEARNY** by Group 4 Web Development Project. All rights reserved.

LEARNY was designed and developed with dedication by:
- Sunera Samuditha
- Achintha Dilhara
- Dilum Piumantha
- Chenuli Ranasinghe
- Nethmi Senarathna

We hope LEARNY enhances the online learning experience for both students and instructors!

---

## Additional Notes

- Ensure **Apache** and **MySQL** are running in XAMPP.
- For any issues or bugs, refer to the logs in the `logs/` directory.
- Keep your **config/** files secure, especially when deploying to a live server.

---

Thank you for choosing LEARNY as your online learning solution!
