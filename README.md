[![PHP](https://img.shields.io/badge/Backend-PHP-777bb4?logo=php)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/Database-MySQL-blue?logo=mysql)](https://www.mysql.com/)
![phpGrid](https://img.shields.io/badge/UI-phpGrid-orange)
[![Status](https://img.shields.io/badge/Stage-Development-yellow)]()

# 🗂️ Customer Relationship Management (CRM) System  

A **web-based CRM** built with **PHP, MySQL, and phpGrid** to streamline customer lifecycle management. It enables sales representatives to track tasks and opportunities, while managers monitor performance and oversee the entire sales pipeline.  

---

## ✨ Features  

### 👩‍💼 Sales Representatives  
- View and manage assigned tasks  
- Add new tasks for leads  
- Convert leads into opportunities  
- Log calls, meetings, and follow-ups  
- Close deals efficiently  

### 👨‍💼 Sales Managers  
- Manage customer accounts and contacts  
- Oversee team activities and task completion  
- Track opportunities and conversions  
- View performance dashboards  

---

## 🏗️ Core Components  

- **Leads** → Initial contacts  
- **Accounts** → Company-level details  
- **Contacts** → Individuals tied to accounts  
- **Opportunities** → Qualified sales prospects  
- **Activities** → Tasks, meetings, calls, and emails  
- **Dashboard** → Visual overview of pipeline  
- **Authentication** → Role-based login (Sales Rep/Manager)  

---

## ⚙️ System Requirements  

- PHP **5.3+**  
- MySQL / MariaDB  
- phpGrid library  

---

## 🗄️ Database Design  

Main tables:  
- `contact` → Stores customer data  
- `notes` → Logs sales activities  
- `users` → Stores login info and roles  

Lookup tables: `contact_status`, `task_status`, `user_status`, `todo_type`, `todo_desc`, `roles`.  

---

## 📊 Database Schema  

![alt text](https://github.com/Hollow27/CRM-System-WebApp/blob/master/database/database%20table%20diagram.png)  

---

## 🚀 Setup  

1. Clone repository  
   ```bash
   git clone https://github.com/your-username/CRM-System.git
   cd CRM-System
Create a MySQL schema (e.g., crm_database).

Import SQL script:

sql
Copy code
SOURCE db/install.sql;
Configure phpGrid in conf.php:

php
Copy code
define("PHPGRID_DB_HOSTNAME","localhost");
define("PHPGRID_DB_USERNAME","root");
define("PHPGRID_DB_PASSWORD","password");
define("PHPGRID_DB_NAME","crm_database");
define("PHPGRID_DB_TYPE","mysql");
define("PHPGRID_DB_CHARSET","utf8");
📑 Application Pages
Tasks Page → Current tasks with statuses

Leads Page → All active leads with details

Opportunities Page → Qualified leads ready for conversion

Customers / Won Page → Closed deals

Manager Dashboard → Tabbed view for sales and team tracking

📌 Future Enhancements
Email notifications

Advanced analytics

Multi-language support

Exportable reports

👨‍💻 Author
Pradeep Rajput
🔗 GitHub | LinkedIn
