# PHP E-Commerce Website 

## Introduction
This is a fully functional e-commerce website built using PHP and MySQL, designed to provide a shopping experience. The platform supports user authentication, product management, cart functionality, order processing, and payment integration.

## Features
- User Registration & Authentication
- Product Listing & Search
- Shopping Cart & Checkout
- Order Management System
- Admin Panel for Product & User Management
- Secure Payment Gateway Integration

## Prerequisites
Before installing, ensure you have the following:
- XAMPP Server (Apache, MySQL, PHP)
- PHP
- MySQL
- phpMyAdmin (for database management)

## Installation & Setup

### 1. Clone the Repository
```sh
git clone https://github.com/sumaiyashah27/Ecommerce-PHP.git
cd Ecommerce-PHP
```

### 2. Configure Database
1. Start **XAMPP** and ensure Apache and MySQL services are running.
2. Open **phpMyAdmin** (`http://localhost/phpmyadmin/`).
3. Create a new database named `shop_db`:
```sql
CREATE DATABASE shop_db;
```
4. Import the provided SQL file:
   - Click on the database `shop_db`.
   - Go to the **Import** tab and upload `database/shop_db.sql`.

### 3. Configure Database Connection
Modify the `config.php` file to match your XAMPP settings:
```php
<?php
$servername = "localhost";
$username = "root";
$password = ""; // Default is empty in XAMPP
$dbname = "shop_db";
$conn = new mysqli($servername, $username, $password, $dbname);
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
```

### 4. Start the Server
1. Move the `Ecommerce-PHP` folder to `htdocs` inside your XAMPP installation.
2. Open XAMPP Control Panel and start **Apache** and **MySQL**.
3. Open your browser and visit:
   ```
   http://localhost/Ecommerce-PHP/
   ```

## Troubleshooting
- Ensure XAMPP’s Apache and MySQL services are running.
- If you see a database connection error, verify `config.php` settings.
- If the site does not load, ensure the project folder is inside `htdocs`.
- Check for errors in `error_log` or enable debugging in `php.ini` by setting `display_errors=On`.

## 📧 Contact
For any queries or support, feel free to reach out:
-  **Email:** [sumaiyashah647@gmail.com](mailto:sumaiyashah647@gmail.com)
-  **LinkedIn:** [Sumaiya Shah](https://www.linkedin.com/in/sumaiya-shah-7a0706224/)
