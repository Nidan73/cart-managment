# 🛒 QuickCart – Desktop E-Commerce Management System

QuickCart is a **C# WinForms desktop-based e-commerce management system** built using **SQL Server**.  
It supports **Admin**, **Seller**, and **Customer** roles with a complete flow from **product management → cart → checkout → order → delivery tracking**.

This project demonstrates real-world concepts such as **role-based access**, **transaction-safe checkout**, **inventory management**, and **relational database design**.

---

## 📌 Features

### 🔐 Authentication & Authorization
- Secure login system with role-based routing
- User roles:
  - **Admin**
  - **Seller**
  - **Customer**
- Account activation control (`IsActive`)

---

### 🧑‍💼 Admin Module
- Admin Dashboard
- Manage Sellers
- Manage Customers
- Manage Products
- Manage Orders
- View all orders placed by customers
- Safe order deletion (handles related OrderItems & Deliveries)

---

### 🏪 Seller Module
- Seller Dashboard
- Add / Update / Delete Products
- Stock management
- View Orders related to seller products
- Shipping & Delivery management
- Update delivery status (`Pending`, `Delivered`)
- Seller Profile Management

---

### 🧑‍🛒 Customer Module
- Customer Dashboard
- Browse Products
- Add products to Cart
- Cart Management
- Checkout system
- Order history
- Customer Profile Management

---

### 🛍 Cart & Checkout Logic
- Stock is **deducted when product is added to cart**
- Stock is **restored when item is removed from cart**
- Cart states:
  - `Active`
  - `CheckedOut`
- Checkout is **transaction-safe**
- Prevents double checkout
- Orders are created only on checkout

---

### 📦 Order & Delivery Flow
- Orders created after checkout
- OrderItems stored per order
- Delivery record auto-created
- Delivery status tracking
- Admin & Seller visibility

---

## 🗄 Database Design

**Database:** `cart_management`  
**DBMS:** Microsoft SQL Server (SSMS)

### Core Tables
- `Users`
- `Customers`
- `Sellers`
- `Products`
- `Carts`
- `CartItems`
- `Orders`
- `OrderItems`
- `Deliveries`

### Key Concepts Used
- Primary Keys & Foreign Keys
- Identity columns
- Transaction handling
- One-to-Many relationships
- Data integrity enforcement

---

## 🛠 Technologies Used
- **C# (.NET Framework)**
- **Windows Forms**
- **SQL Server**
- **SQL Server Management Studio (SSMS)**
- **ADO.NET**

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/QuickCart.git
