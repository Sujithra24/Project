                                                               User Registration and Validation

This project is a user registration system built with HTML, CSS, JavaScript, PHP, and MySQL (XAMPP). It allows users to register their information securely and stores it in a database.

Why Bootstrap is Used

Bootstrap is used in this project to:
.Make the form responsive, so it looks good on desktop, tablet, and mobile.
.Provide modern styling without writing a lot of custom CSS.
.Use prebuilt components like buttons, form fields, and alerts for a clean design.
.Save development time while keeping the layout professional.

What this Project Does
Displays a registration form for the user to fill:

First Name
Last Name
Gender
Phone Number
Email
Password

When submitted:
.Validates the input using JavaScript and PHP.
.Hashes the password for security.
.Stores all information in a MySQL database (XAMPP).
.The form disappears after successful registration, showing a success message.

How it Works:
1. Front-end (HTML + CSS + Bootstrap + JS)
.index.html → Shows the form.
.style.css → Custom styling.
.script.js → Handles client-side validation and AJAX submission.

2. Back-end (PHP)
.process.php → Handles server-side validation, hashes passwords, and inserts data into MySQL.

3. Database (MySQL via XAMPP)
.Database name: sign
.Table name: sign

Stores user information:
firstName
lastName
gender
number
email
password (hashed)

File Structure:

 user registration-form/
│
├── index.html      # Registration form
├── style.css       # Custom CSS styling
├── script.js       # JavaScript for validation and AJAX
├── process.php     # PHP backend to process form and insert data
└── README.md       # Project documentation

Database Setup:
1. Open XAMPP → Start Apache and MySQL.
2. Open phpMyAdmin → Create a database called sign.
3. Create a table sign using the following SQL:

CREATE TABLE sign (
    id INT AUTO_INCREMENT PRIMARY KEY,
    firstName VARCHAR(50),
    lastName VARCHAR(50),
    gender ENUM(10),
    number BIGINT (20),
    email VARCHAR(50),
    password VARCHAR(20)
);

How to Use:
1. Place all project files Xampp inside htdocs (or a folder inside it).
2. Open index.html in your browser.
3. Fill out the registration form and submit.
4. On successful registration:

The form disappears.
 A “Registration successful!” message is displayed.
  
"Your data is stored in the MySQL database (sign table)."

5. You can check registered emails and details in phpMyAdmin.

Technologies Used:
.HTML → Structure of the form
.CSS → Custom styling
.Bootstrap  → Responsive design, modern styling, and components
.JavaScript → Client-side validation and AJAX submission
.PHP → Server-side validation and database insertion
.MySQL (XAMPP) → Storing registered users securely

Security Features:
.Passwords are hashed using password_hash() before storing in the database.
.Client-side validation improves user experience.
.Server-side validation ensures data integrity and prevents invalid entries.

Future Improvements:
.Check for duplicate email addresses before registration.
.Add password strength meter.

Add email verification and login system.

Add a dashboard to view registered users.
