# 📁 File Hider – Java Project

## 🔒 Description

**File Hider** is a Java-based desktop application that allows users to securely **hide and unhide files** using a simple interface and secure authentication. It implements **OTP-based email verification** to ensure user identity during **login** and **sign-up**. Files are stored securely in a database and can be restored as needed.

---

## ✨ Features

- ✅ **OTP-based Authentication**
    - Implements email-based One-Time Password (OTP) verification for both sign-up and login.
    - Uses `javax.mail` to send OTPs securely to the user's email.

- 📂 **File Management**
    - Uses `ArrayList` to manage and display the list of hidden files per user session.
    - Displays hidden files associated with a logged-in user.

- 🛡️ **File Hiding Logic**
    - Reads file data using `FileReader` and stores it in a MySQL database using CLOB (`bin_data`).
    - Deletes the original file from the system to ensure privacy.

- 📤 **Unhiding Files**
    - Retrieves file data from the database, recreates the original file, and deletes the record from the database.

---

## 🛠️ Technologies Used

- **Java (Core, I/O, JDBC)**
- **JavaMail API** – For sending OTPs via email.
- **MySQL** – For storing user data and file contents.
- **JDBC** – For performing SQL operations like insert, retrieve, and delete.

---
