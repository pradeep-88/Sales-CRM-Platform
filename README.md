[![PHP](https://img.shields.io/badge/Backend-PHP-777bb4?logo=php)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/Database-MySQL-blue?logo=mysql)](https://www.mysql.com/)
![phpGrid](https://img.shields.io/badge/UI-phpGrid-orange)
[![Status](https://img.shields.io/badge/Stage-Development-yellow)]()

# 🗂️ Customer Relationship Management (CRM) System  

This project is a **web-based CRM application** built with **PHP, MySQL, and phpGrid**. It helps sales teams and managers track leads, manage opportunities, and monitor sales performance through an intuitive interface. The system is lightweight, role-based, and easy to deploy.  

---

## ✨ Features  

### 👩‍💼 For Sales Representatives  
- View and update assigned tasks  
- Add new tasks for specific leads  
- Convert qualified leads into opportunities  
- Record sales activities such as calls, emails, and meetings  
- Close deals and update customer status  

### 👨‍💼 For Sales Managers  
- Manage customer accounts and contact details  
- Oversee team activities and task completion  
- Track ongoing opportunities and closed deals  
- Access performance dashboards for quick insights  

---

## 🏗️ Core Components  

- **Leads** → Initial customer contacts  
- **Accounts** → Company-level information  
- **Contacts** → Individual customer or business representatives  
- **Opportunities** → Qualified sales leads  
- **Activities** → Tasks, calls, meetings, and emails  
- **Sales** → Team members managing customer lifecycle  
- **Dashboard** → Visual overview of sales pipeline and activities  
- **Authentication** → Role-based login for managers and reps  

---

## ⚙️ System Requirements  

- PHP **5.3+**  
- MySQL / MariaDB  
- phpGrid library  

---

## 🗄️ Database Design  

The CRM database follows a relational model with the following main tables:  

- `contact` → Stores customer information (name, company, project details)  
- `notes` → Records activities such as meetings and calls  
- `users` → Contains login details and assigned roles  

Additional lookup tables:  
- `contact_status` → Lead, Opportunity, or Customer  
- `task_status` → Pending or Completed  
- `user_status` → Active or Inactive  
- `todo_type` → Task or Meeting  
- `todo_desc` → Task details (e.g., Follow-up Email, Call)  
- `roles` → Defines Manager or Sales Rep access  

---

## 📊 Database Schema  

![alt text](https://github.com/Hollow27/CRM-System-WebApp/blob/master/database/database%20table%20diagram.png)  

The diagram above illustrates table relationships, primary keys, and role-based structure for managing sales activities.  

---

## 🚀 Setup  

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/CRM-System.git
   cd CRM-System
