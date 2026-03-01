# S2.03 — MongoDB Data Structure

## 🎯 Objectives
This project focuses on practicing NoSQL data modeling with MongoDB through hands-on exercises inspired by real-world business cases.

## 📌 Level 1 — Optical Store
- **Exercise 1**  — Customer-Oriented Model

In this version, the system is structured around the customer as the main entity.

The database must support:

- Customer personal information and registration date
- Referral relationship (which customer recommended another) 
- Customer sales history
- Employee responsible for each sale
- Date and time of each sale
- Glasses sold (brand, frame type, colors, lens prescription, price)
- Supplier information related to each pair of glasses

This perspective prioritizes customer queries and purchase tracking.

- **Exercise 2** — Glasses-Oriented Model

In this version, the database is designed with glasses as the core entity.

The model must allow:

- Viewing glasses as the primary document
- Identifying their supplier
- Tracking all related sales
- Linking sales with customers
- Associating employees with each sale
- Storing timestamps for transactions
- This approach is useful when inventory and product management are the primary focus.

## 📌 Level 2 — Food Delivery System
- **Exercise 1** — Online Food Ordering Platform

Design a MongoDB database for an online food delivery system with the following requirements:

- Customers can place multiple orders
- Each order belongs to one customer and one store
- Orders may contain multiple products (pizzas, burgers, drinks)
- Orders must store:
- Date and time
- Delivery or pickup type
- Product quantities
- Total price
- Optional notes
- Stores manage multiple orders
- Employees work for a single store

Delivery orders must include:

- Assigned delivery employee
- Delivery date and time
- Pizzas belong to categories that may change over time

This exercise reinforces modeling decisions involving nested documents, references, and evolving data structures.

## 🛠 Technologies Used

- MongoDB
- MongoDB Compass
- Docker 
- Moon Modeler (ER diagrams and JSON schema design)
- Git & GitHub

## 🚀 Installation and Execution

1. **📂Clone the repository**:
   `git clone https://github.com/carlasalmeron/S2.03-MongoDB-Data-Structure.git`

2. **Setup environment:** Start the environment (Docker): docker run -d -p 27017:27017 --name mongodb mongo

3. **Import the JSON Script:**
- MongoDB Compass:
- Connect to `mongodb://localhost:27017`
- Create the database
- Import the `s.json` file into the corresponding collections
