# Furniture Store Database Conceptual Model
# 📌 Project Overview

This project focuses on designing a conceptual database model for a furniture store management system. The objective is to translate real-world business processes into a structured data model that supports key operational activities such as product management, customer orders, quotations, payments, and inventory tracking.

The model captures relationships between core business entities and ensures that the system reflects realistic business rules and workflows used in retail operations.

# 🧠 Objectives

- Translate real-world business rules into a conceptual data structure

- Design an Entity-Relationship Model (ERD) representing key business entities

- Define relationships between customers, products, orders, quotes, and payments

- Support essential retail business processes such as order placement, quotation generation, and payment allocation

# 📊 Conceptual Model Design

### Core entities:

- Customer: CustomerID (PK), CustomerName, ContactName, CustomerPhone, CustomerAddress

- Customer Type: CustomerTypeID (PK), CustomerTypeName, CustomerTypeDescription

- Furniture Item: FurnitureItemID (PK), ReferenceString, ItemCostPrice, ItemSalePrice, ItemDescription, ItemLocationString, ItemStockQuantity

- Category (parent-child relationships): CategoryID (PK), CategoryName, CategoryDescription

- Product Type: ProductTypeID (PK), ProductName

- Request: RequestID (PK), RequestDate, RequestTime, RequestDescription

- Quote: QuoteID (PK), QuoteDate, QuoteTime, QuoteDescription

- Order: OrderID (PK), OrderDate, OrderTime, DeliveryInstructions

- Payment: PaymentID (PK), PaidAmount, PaymentDate, PaymentTime, PaymentMethod, ExternalRefNo

- Staff: EmployeeID (PK), EmployeeName, EmployeeRole, EmploymentType

- Resource: ResourceID (PK), ResourceName, ResourceDescription

- Resource Type: ResourceTypeID (PK), ResourceTypeName, ResourceTypeDescription

### Supporting entities

- Requested Item

- Quote Item

- Order Item

- Quoted Order Item

- Furniture Order Item

- Requested Item Resource

- Payment Allocation

These entities help represent transaction-level relationships and dependencies within the system.

<img width="1460" height="866" alt="Image" src="https://github.com/user-attachments/assets/06f96dd5-9f8b-49e0-9cd5-f1e5d1909c18" />

# 🖇️ Data Relationships

Customer → Request → Quote → Order

Order → Order Item → Furniture Item

Furniture Item → Category / Product Type

Order → Payment → Payment Allocation

This relational structure supports transaction tracking, inventory management, and financial records.

# 🔎 Tools Used

Draw.io – Database conceptual modelling

Entity Relationship Diagram (ERD) methodology

Business rule analysis

