# 🏬 Mall Management System

This is a terminal-based **Mall Management System** project developed in **Python** with **MySQL** as the backend. It simulates the management structure and billing processes of a mall, providing functionality for different user roles.

---

## 👤 User Roles

### 1. **Admin**
- Full access to the system
- Can create, modify, and delete:
  - Customer and employee records
  - Passwords and personal details

### 2. **Customer**
- Can **Sign Up** to receive a unique **Customer ID**
- Each visit generates a new **Bill ID**
  - Multiple Bill IDs allowed per customer
- Can view their **previous bills** by selecting bill creation dates
- Cannot **logout** until all bills are paid
- Can view closed bill details (read-only) but cannot add new purchases to them

### 3. **Cashier**
- Employees of the mall
- Can view **Customer IDs** and their active **Bill IDs**
- Handles **payment and bill closing**

---

## 🛠 Technologies Used
- **Frontend**: Python (CLI interface)
- **Backend**: MySQL
- **Library**: `mysql-connector-python`

---

## ⚙️ Features
- User authentication for all roles
- Self-initializing database setup on first run
- Itemized billing system
- Role-based access control
- Clean separation of duties between admin, customer, and cashier
- Historical bill viewing by date
- Auto-bill lock once payment is done

---

## 🚀 How to Run

1. Ensure MySQL is installed and running on your system.
2. Install required Python module:
   ```bash
   pip install mysql-connector-python
