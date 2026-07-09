🍽️ Spice Garden — Restaurant Management System
A desktop restaurant management application built with Java Swing (GUI) and MySQL/JDBC (persistence). It supports role-based dashboards for Managers, Chefs, Waiters, and Receptionists, covering the full restaurant workflow — menu management, inventory, table reservations, order processing, billing, payments, and employee management.
✨ Features
Role Selection — Manager, Chef, Waiter, Receptionist dashboards
Menu Management — add, view, and remove menu items (stored in MySQL)
Inventory Management — track ingredients, quantities, thresholds, and restocking
Table & Reservation Management — allocate tables, make reservations/walk-ins, free tables
Order Management — create orders, add items, track status (Pending → Confirmed → Preparing → Ready → Delivered)
Billing & Payments — generate bills, process payments (Cash/Card/UPI/Wallet), handle partial payments and refunds
Employee Management — add/remove Chefs, Waiters, and Managers; track past employees
Reports — order stats, revenue, table occupancy, and employee summaries
Daily Revenue Dashboard — total revenue, average order value, top-selling items
🛠️ Tech Stack
Language: Java
GUI: Java Swing (CardLayout-based navigation)
Database: MySQL (via JDBC)
Architecture: DAO pattern for database access (OrderDAO, BillDAO, PaymentDAO, ReservationDAO, RestaurantTableDAO, CustomerDAO)
📋 Prerequisites
JDK 17+ (or compatible version)
MySQL Server running locally
MySQL Connector/J (JDBC driver) on the classpath
⚙️ Setup
Install and start MySQL Server.
Create the database:

CREATE DATABASE spice_garden;

Update database credentials in the source (DBConfig, DatabaseIntegration, etc.) if different from the defaults.
Compile and run:

javac Main.java

java Main

Required tables (menu_items, ingredients, restaurant_tables, reservations, orders, etc.) are created automatically on first run.
🚀 Usage
Launch the app and click Enter on the welcome screen.
Select a role:
Manager — manage menu, inventory, employees, and view reports/revenue
Receptionist — handle table reservations and walk-ins
Chef — view and update order status
Waiter — create orders, mark deliveries, generate bills, process payments
📌 Notes
Database credentials are currently hardcoded for local development — replace with environment variables or a config file before deploying or sharing publicly.
This project is intended as a learning/demo application for restaurant workflow management.
📄 License
MIT License (or specify your preferred license).
