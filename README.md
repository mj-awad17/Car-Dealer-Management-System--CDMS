# 🚗 Car Dealer Management System (CDMS) – Microsoft Access RDBMS

A complete Relational Database Management System (RDBMS) for a medium-sized car dealership, built in Microsoft Access to manage cars, customers, sales, staff, and services in a reliable, scalable, and structured way.

---
<!-- <p align="center">
  <img style='border-radius:15px', src="https://github.com/mj-awad17/Car-Dealer-Management-System--CDMS/blob/main/Banner-car-management-system.png" alt="Car Dealership Management System Banner" width="100%">
</p> -->

<p align="center">
  <img
    src="https://github.com/mj-awad17/Car-Dealer-Management-System--CDMS/blob/main/Banner-car-management-system.png"
    alt="Car Dealership Management System Banner"
    style="border-radius: 18px; max-width: 100%; height: auto;"
  />
</p>


## ✨ Project Overview

This project replaces manual spreadsheets and handwritten logs with a fully normalized Microsoft Access database tailored for car dealership operations.  
The system supports inventory control, customer management, sales tracking, staff performance monitoring, and vehicle service history in one integrated solution.

---

## 🎯 Key Features

- 🔐 **Relational MS Access Database** with clearly defined tables and relationships  
- 📊 **Entities:** Cars, Customers, Sales, Staff, Services  
- 📚 **Fully normalized to 3NF** to improve consistency and reduce redundancy  
- ✅ **Primary and Foreign Keys** with referential integrity enforced  
- 🧪 **Validation rules** for IDs, dates, prices, mileage, and contact info  
- 🧾 **10–15 realistic records per table** to simulate real dealership data  
- 🔎 **Business-focused SQL queries** for reporting and analytics  
- 🖥️ **User-friendly forms** for CRUD operations (no direct table editing needed)  
- 🔒 **Basic privacy, security, and GDPR-aligned practices** for personal data

---

## 🧱 Database Design

### Entities & Relationships

The core data model is structured around these main entities:

- **Cars** – Vehicle inventory (new and used), including make, model, year, colour, mileage, fuel type, transmission, price, status, and purchase date.  
- **Customers** – Customer profiles including name, address, city, postcode, phone, and email.  
- **Sales** – Records of completed sales linking cars, customers, and staff, including sale date, sale price, and payment method.  
- **Staff** – Staff members involved in sales and service operations, with job titles and contact info.  
- **Services** – Service and maintenance jobs including service type, date, cost, and notes.

Key relationships (implemented with PK/FK constraints):

- One **Customer** → Many **Sales**  
- One **Car** → One **Sale**  
- One **Car** → Many **Services**  
- One **Staff** → Many **Sales**  
- One **Staff** → Many **Services**

### Normalization & Integrity

- All tables are designed in **Third Normal Form (3NF)** to eliminate repeating groups, partial dependencies, and transitive dependencies.  
- Each table has a dedicated **Primary Key** (CarID, CustomerID, StaffID, SaleID, ServiceID) using AutoNumber/Integer.  
- **Foreign Keys** connect Sales to Cars, Customers, and Staff; and Services to Cars and Staff.  
- Referential integrity is enforced so no sale or service exists without valid related records.

---

## 🛠️ Implementation Details

### Tech Stack

- 🗄️ **Microsoft Access 2019/2021** – database, queries, and forms  
- 📐 **ERD Tool (e.g., Draw.io)** – conceptual and logical data modeling  
- 🧩 **SQL (MS Access Query Designer)** – query development and reporting  
- 💻 **Windows OS** – runtime platform

### Tables & Sample Data

Each core table contains **10–15 realistic records** to reflect real-world usage:

- **Cars** – mixture of new and used vehicles with realistic attributes  
- **Customers** – individuals from different locations and contact details  
- **Sales** – purchase records referencing valid cars, customers, and staff  
- **Staff** – sales and workshop personnel with roles and contact info  
- **Services** – maintenance and repair jobs with service type and cost

---

## 🔍 Business Queries & Reports

The system includes at least **10 analytical SQL queries**, such as:

- 🚘 Cars currently **available for sale**  
- 📅 **Sales ordered by date** for performance tracking  
- 👨‍💼 **Sales by staff member** for performance evaluation  
- 💰 **Total sales revenue** summary  
- 🛠️ **Cars with service history** and last service date  
- 🧍 **Customer purchase history** (loyalty/retention insight)  
- 📦 **Car stock summary** (sold vs available)  
- 💸 **Total service cost** summary  
- 📅👨‍💼 **Sales by date and staff member**  
- 📋 **Full sales listing query** for audits and exports

These queries help management monitor revenue, stock, operational expenses, and staff performance.

---

## 🖥️ Application Interface (Forms)

To make the system accessible to non-technical users, the project includes user-friendly **MS Access forms**:

- **Customer Form** – Add, edit, and navigate customer records  
- **Cars Form** – Manage inventory and car details  
- **Sales Form** – Record and review sales transactions  
- **Staff Form** – Maintain staff information and job roles  
- **Services Form** – Log vehicle services and maintenance history  

Each form supports:

- Add new record  
- Save record  
- Navigate through existing records (first/previous/next/last)

---

## 🔐 Privacy, Security & Compliance

### GDPR & Ethics

- Collects and stores **only necessary personal data** (data minimization principle)  
- Data is used strictly for **legitimate business purposes**  
- No misuse of customer or staff contact information  
- Service and operational data is kept confidential

### Security Measures

- Optional **database password protection**  
- Use of **ACCDE packaging** to protect design and logic from modification  
- Recommended **regular backups** and secure storage locations  
- Optional encryption of sensitive fields (e.g., contact info)

---

## ⚠️ Limitations & Future Work

### Current Limitations

- MS Access is not ideal for **very large datasets**  
- Limited **multi-user concurrency** and scalability  
- Windows-only environment  
- Forms are functional but **UI/UX is basic**

### Future Enhancements

- Migrate to **SQL Server** or **MySQL** for better scalability and concurrency  
- Develop a **web-based front-end** (e.g., ASP.NET, Django, Node.js)  
- Implement **role-based access control** and activity logs  
- Add **interactive dashboards** and advanced analytics (charts, KPIs, trends)

---

## 👨‍💻 Author / Developer

Developed by **Muhammad Jawad** – Database Designer & Developer.  

🔗 **Connect on LinkedIn:** [mjawad17](https://www.linkedin.com/in/mjawad17/)

⭐ If you find this project helpful, feel free to star, fork, and adapt it for your own academic or professional use!
