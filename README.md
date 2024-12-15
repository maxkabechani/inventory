# Inventory Management

A Laravel and Vue.js Inventory Management System.

---

## Description

This is a web application built using Laravel as the backend framework and Vue.js for the frontend developed by Max Kabechani. The project is designed to deliver seamless interaction between the server-side logic and client-side UI. It is ideal for creating modern, dynamic web applications.

---

## Features

- Dynamic frontend using Vue.js
- RESTful API powered by Laravel
- Seamless integration between backend and frontend
- Modular and scalable architecture

---

## Installation

Follow these steps to set up the project on your local machine:

### Prerequisites

1. **Download Repository**
    - Download the repository
2. **Install XAMPP Server**
   - Download and install XAMPP from the [official website](https://www.apachefriends.org/).
   - Start the Apache and MySQL services in XAMPP.

   #### Install XAMPP via Install XAMPP

   **Step 1**: Move the inventory folder to `C:/xampp/htdocs/`.

   **Step 2**: Go to `C:\Windows\system32\drivers\etc\` and open the "hosts" file in Administrator mode. Add the following code to it:

   ```
   127.0.0.1 inventory.local
   ```

   **Step 3**: Navigate to `C:\xampp\apache\conf\extra` and open the `httpd-vhosts.conf` file. Add the following code:

   ```
   <VirtualHost inventory.local:80>
       ServerAdmin webmaster@inventory.local
       DocumentRoot "C:/xampp/htdocs/inventory"
       ServerName www.inventory.local
       ServerAlias inventory.local

       <Directory "C:/xampp/htdocs/inventory">
           Options Indexes FollowSymLinks Includes ExecCGI
           AllowOverride All
           Require all granted
       </Directory>

       ErrorLog "logs/inventory.local-error.log"
       CustomLog "logs/inventory.local-access.log" common
   </VirtualHost>
   ```

   **Step 4**: Restart XAMPP.

   **Setup Installation**: Access the URL `http://inventory.local/setup`.

## Technologies Used

- **Laravel**: PHP framework for backend development.
- **Vue.js**: JavaScript framework for building user interfaces.
- **XAMPP**: Local server environment.
- **Node.js**: Runtime environment for JavaScript.
- **Composer**: Dependency manager for PHP.
