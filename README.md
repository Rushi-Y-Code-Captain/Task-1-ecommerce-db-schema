#  E-commerce Database Schema

##  Task 1: Database Setup and Schema Design

This repository contains the SQL script and ER diagram for setting up a simple **E-commerce** database. 
It is created as part of Task 1 to learn how to:
- Create databases and tables
- Define primary and foreign keys
- Design entity relationships

##  Domain

**Domain Chosen:** E-commerce

Entities and relationships are designed for a basic online shopping platform.

##  Entities

| Entity       | Attributes |
|--------------|-------------|
| **Customer** | customer_id (PK), name, email, address |
| **Product**  | product_id (PK), name, description, price |
| **OrderTable** | order_id (PK), order_date, customer_id (FK) |
| **OrderItem** | order_item_id (PK), quantity, order_id (FK), product_id (FK) |

##  Relationships

- **Customer** → **OrderTable** : One-to-Many  
- **OrderTable** → **OrderItem** : One-to-Many  
- **OrderItem** → **Product** : Many-to-One

##  Files

- `schema.sql` — SQL script to create the tables and constraints.
- `er_diagram.png` — Visual ER Diagram showing entities and relationships.

##  How to Use

1. Open MySQL Workbench / pgAdmin / SQLiteStudio.
2. Run `schema.sql` to create the tables.
3. Refer to `er_diagram.png` to understand the schema design.

##  Outcome

A well-structured E-commerce database schema with clear entities, relationships, and constraints.

##  Submission

Submit your GitHub repository link as per the instructions.
