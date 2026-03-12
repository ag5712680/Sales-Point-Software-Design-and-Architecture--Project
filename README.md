# Sales-Point-Software-Design-and-Architecture--Project
 #  A modular sales management platform developed with a focus on Software Design & Architecture (SDA) principles and robust documentation.
  #  Project OverviewThe Sales Point system :
  is designed to automate day-to-day sales operations, including managing products, customers, carts, orders, and payments. It aims to solve common issues like inaccurate inventory, slow billing, and scattered order records.
 #  Architectural Design
 This project implements a hybrid architectural approach for scalability and maintainability:
 # Layered Architecture:
  Divided into Presentation (UI), 
  Application (Business Logic),
  Data Access, 
  Database layers.
#  Repository Architecture:
   Uses a central database as the "single source of truth" to ensure data consistency across Admin and Customer roles.
 #  S.O.L.I.D Principles 
 AppliedTo ensure a flexible and maintainable design, I followed all five SOLID principles:
 #  Single Responsibility (SRP): 
 Every class (e.g., Customer, Product, Payment) has a single, clear responsibility.
  # Open/Closed (OCP): 
 New modules like discounts or payment methods can be added without modifying core logic.
  # Liskov Substitution (LSP):
  Admin, Customer, and Employee roles correctly inherit from the base User class.
  # Interface Segregation (ISP): 
 Actors only interact with relevant functions, avoiding bloated classes.
   Dependency Inversion (DIP):
  Minimal direct dependencies; for example, Order interacts with products via OrderItem.
   #  Design Patterns ImplementedCreational:
  # Singleton Patterns :
    for database connections and Factory for creating user roles (Admin/Customer).
   # Structural: 
   Facade for simplifying UI interactions and Adapter for converting raw database records into display objects.
   #  Behavioral: 
   Observer for real-time inventory updates and Command for handling UI button actions.
 #  Key FeaturesRole-Based Access: 
 Separate dashboards and functionalities for Admin, Customers, and Employees.
 # Inventory Control:
 Admin can add, update, or delete products and monitor stock levels.
#  Smooth Checkout:
Cart management, multiple payment options (Cash/Card/Online), and automated invoice generation.
#  Customer Support: 
Integrated complaint registration and response system
