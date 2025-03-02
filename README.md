# 🏦 Insurance Database Management System

## 📌 Project Overview  
This project is a **Database Management System (DBMS)** implementation for **SAME**, an insurance company that provides coverage to **domestic and international passengers**. As the company expanded, manually managing data became inefficient.  

This project introduces a **relational database system** to efficiently store, update, and manage data related to **passengers, flights, insurance policies, payments, and agents**.  

The **database is designed using Oracle SQL**, and the **web application** is built with **Node.js and React.js** for seamless user interaction.  

---

## 🚀 Key Features  
✅ **Ternary Relationship Model** – Efficiently maps relationships between passengers, flights, and insurance policies.  
✅ **Normalization & Redundancy Reduction** – Uses **foreign keys** to reduce redundancy, particularly for agents.  
✅ **User-Friendly Web Application** – Built using **React.js** and **Node.js** for a dynamic user interface.  
✅ **Security Implementation** – **SQL Injection** prevention techniques included.  
✅ **Payment & Invoice Management** – Allows **multi-card payments** per booking.  

---

## 🛠 Tech Stack  

### **Database**  
![Oracle](https://img.shields.io/badge/Oracle_SQL-F80000?style=for-the-badge&logo=oracle&logoColor=white)  

### **Backend**  
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)  
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)  

### **Frontend**  
![React](https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=black)  

### **Libraries**  
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)  
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)  

---

## 📊 Database Design  

### **📌 Summary & Assumptions**  
- **Ternary Relationship**: Passengers, Flights, and Insurance policies are interrelated.  
- **Agents Table**: To avoid redundancy, a separate **Agent Table** stores agent details.  
- **Passengers' Preferences**: Cabin class, meal plan, and special requests are recorded.  
- **Payments**: A single invoice may be paid using multiple payment methods.  
- **Airports & Airlines**: Have a **many-to-many** relationship.  

### **📌 Logical & Relational Model**  
- **Normalization**:  
  - `Agents` are referenced via `agentID` to eliminate duplicate data.  
  - `Passengers` may not always have a **passport** (domestic flights allow local IDs).


## 📌 Security Features
✅ SQL Injection Prevention – Uses parameterized queries to prevent unauthorized access.
✅ User Authentication – Ensures only authorized users can access certain data.


## 📸 Work Samples

### 🔹 Screenshot 1: Login Page
![Login Page](https://github.com/kiran98118/Insurance-Management-System/blob/e532e788d0e831895d9ac969d5df5e6d4835ac26/Images/Screen%20Shot%202025-03-02%20at%202.22.25%20PM.png?raw=true)

### 🔹 Screenshot 2: User details in the Database
![Dashboard](https://github.com/kiran98118/Insurance-Management-System/blob/e532e788d0e831895d9ac969d5df5e6d4835ac26/Images/Screen%20Shot%202025-03-02%20at%202.21.34%20PM.png?raw=true)

### 🔹 Screenshot 3: Payment details in the Database
![Dashboard](https://github.com/kiran98118/Insurance-Management-System/blob/e532e788d0e831895d9ac969d5df5e6d4835ac26/Images/Screen%20Shot%202025-03-02%20at%202.21.46%20PM.png?raw=true)



