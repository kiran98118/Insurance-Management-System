# Insurance Database Management System

## Project Overview  
This project is a Database Management System (DBMS) implementation for SAME, an insurance company that provides coverage to domestic and international passengers. As the company expanded, manually managing data became inefficient. This project introduces a relational database system to efficiently store, update, and manage data related to passengers, flights, insurance policies, payments, and agents.

The database is designed using Oracle SQL, and the web application is built with Node.js and React.js for seamless user interaction.

---

## Key Features  
- Ternary Relationship Model – Efficiently maps relationships between passengers, flights, and insurance policies.  
- Normalization & Redundancy Reduction – Uses foreign keys to reduce redundancy, particularly for agents.  
- User-Friendly Web Application – Built using React.js and Node.js for a dynamic user interface.  
- Security Implementation – SQL Injection prevention techniques included.  
- Payment & Invoice Management – Allows multi-card payments per booking.  

---


## Tech Stack  
- Database: Oracle SQL  
- Backend: Node.js  
- Frontend: React.js  
- Libraries:  
  - Express.js – Backend API  
  - MySQL2 – Database connection  
  - React.js – Frontend framework  

---

## Database Design  

### Summary & Assumptions  
- Ternary Relationship: Passengers, Flights, and Insurance policies are interrelated.  
- Agents Table: To avoid redundancy, a separate Agent Table stores agent details.  
- Passengers' Preferences: Cabin class, meal plan, and special requests are recorded.  
- Payments: A single invoice may be paid using multiple payment methods.  
- Airports & Airlines: Have a many-to-many relationship.  

### Logical & Relational Model  
- Normalization:  
  - Agents are referenced via agentID to eliminate duplicate data.  
  - Passengers may not always have a passport (domestic flights allow local IDs).  

### SQL DDL (Schema Definition)  
The project uses Oracle SQL to define the database structure.  
Example:
CREATE TABLE ussk_agent ( agent_id NUMBER(3) NOT NULL, agent_fname VARCHAR2(10) NOT NULL, agent_lname VARCHAR2(10) NOT NULL, agent_email VARCHAR2(15) NOT NULL, agent_phoneno VARCHAR2(10) NOT NULL, PRIMARY KEY (agent_id) );


## Installation & Setup  

### Clone the Repository  

### Set Up the Database  
1. Open Oracle SQL Developer or any SQL client.  
2. Run the DDL script from `schema.sql` to create tables.  

### Install Dependencies  
For Backend (Node.js & Express.js): 

## Security Features  
- SQL Injection Prevention – Uses parameterized queries to prevent unauthorized access.  
- User Authentication – Ensures only authorized users can access certain data.  

---
