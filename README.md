<!--
===========================================================
  README.md - Knowledge Haven Library Management System
  GitHub Repository: Library-Haven-Management-System
===========================================================
-->

<h1 align="center">
  <img src="assets/images/logo-library.png" width="50" height="50" alt="Logo">
  <br>
  Knowledge Haven – Library Management System
</h1>

<p align="center">
  <strong>A complete, role‑based web application for managing library operations, built with PHP and MySQL.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.0+-777BB4?style=flat&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/MySQL-8.0+-4479A1?style=flat&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=flat&logo=bootstrap&logoColor=white" alt="Bootstrap">
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Status-Stable-brightgreen" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-blue" alt="License">
</p>

---

## 📖 Overview

**Knowledge Haven** is a feature‑rich library management system designed for both **librarians (employees)** and **library members**. It streamlines book inventory, user management, borrowing/return workflows, fine tracking, and reporting – all through an intuitive, responsive interface.

Whether you are a small community library or a school resource centre, this system helps you keep track of every book, member, and transaction with ease.

---

## 🚀 Key Features

### 🔹 Employee (Librarian) Dashboard
- **📚 Book Management** – Add, edit, delete, search, and view books.
- **✍️ Author Management** – Maintain author records with birth/death years and nationality.
- **🏷️ Category Management** – Organise books by categories (Fiction, Science, History, etc.).
- **📍 Location Management** – Define shelf locations (floor, shelf, code) and mark them active/inactive.
- **👥 User Management** – Activate/deactivate members, view borrowing history, and delete users.
- **🔄 Transaction Management** – Monitor all borrow/return/renew transactions with date filters and sorting.
- **📊 Reports & Analytics** – Overview, books analysis, user activity, and financial summaries with dynamic charts (Chart.js).
- **⚙️ Settings** – Update profile, change password, and manage employee details.

### 🔸 Member Dashboard
- **🔍 Browse Books** – Search by title, author, ISBN, or category; check availability.
- **📖 Borrow Books** – Instantly borrow available books (max 5 active loans) with auto‑generated due dates (14 days).
- **📤 Return Books** – Return borrowed books; overdue fines are calculated automatically ($0.50/day).
- **📜 Transaction History** – View complete borrowing/return history with filters (status, type, month, year).
- **👤 My Profile** – Update personal information, change password, and upload a profile picture.

### ✅ Additional Highlights
- **Secure Authentication** – Role‑based access (employee / member) with hashed passwords.
- **Automated Fine Calculation** – Overdue books incur fines that are tracked per member.
- **Responsive UI** – Built with Bootstrap 5, works on desktop, tablet, and mobile.
- **Profile Image Upload** – Members and employees can upload custom profile pictures.
- **Bulk Actions** – Employees can activate/deactivate or delete multiple users at once.

---

## 🛠️ Technology Stack

| Layer          | Technology                                                                 |
|----------------|----------------------------------------------------------------------------|
| **Backend**    | PHP 8.0+ (procedural with `mysqli`)                                        |
| **Database**   | MySQL 8.0+ (relational schema with foreign keys)                           |
| **Frontend**   | HTML5, CSS3, JavaScript (ES6+)                                             |
| **CSS Framework** | Bootstrap 5.3 (customised with Font Awesome 6.4)                        |
| **Charts**     | Chart.js 4.4 (for reports)                                                 |
| **Icons**      | Font Awesome 6.4                                                            |
| **Fonts**      | Google Fonts (Poppins & Playfair Display)                                  |

---

## 📋 Database Schema (Key Tables)

- **users** – Authentication & profile data (role, email, password, etc.)
- **employees** – Employee‑specific details (employee_code, position, hire_date)
- **members** – Member‑specific details (member_code, fines, total_borrowed)
- **authors** – Author information (name, birth/death year, nationality)
- **categories** – Category names
- **locations** – Physical shelf locations (code, floor, shelf, is_active)
- **books** – Book metadata (title, isbn, copies, availability, description)
- **transactions** – Borrow/return/renew records (member_id, book_id, dates, status)
- **fines** – Fine records linked to transactions (amount, reason, status)

---

## 🧩 Installation Guide

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Library-Haven-Management-System.git
