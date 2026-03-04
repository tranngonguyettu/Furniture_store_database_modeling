# Furniture Store Database Conceptual Model
# Project Overview

This project focuses on designing a conceptual database model for a furniture store management system. The objective is to translate real-world business processes into a structured data model that supports key operational activities such as product management, customer orders, quotations, payments, and inventory tracking.

The model captures relationships between core business entities and ensures that the system reflects realistic business rules and workflows used in retail operations.

# Objectives

- Translate real-world business rules into a conceptual data structure

- Design an Entity-Relationship Model (ERD) representing key business entities

- Define relationships between customers, products, orders, quotes, and payments

- Support essential retail business processes such as order placement, quotation generation, and payment allocation

# Conceptual Model Design

- The conceptual model includes 10+ business entities, representing different components of the furniture store ecosystem.

- Key Entities

Customer – stores customer information and contact details

Customer Type – categorises customers based on classification

Furniture Item – represents products available for sale

Category – groups furniture items into logical categories

Product Type – defines specific product classifications

Request – represents customer requests for product quotations

Quote – generated quotation based on requested items

Order – records confirmed customer purchases

Payment – manages payment transactions

Resource – represents operational resources required to fulfil requests

Supporting transactional entities include:

Requested Item (Weak Entity)

Quote Item

Order Item

Payment Allocation

These entities help represent transaction-level relationships and dependencies within the system.

# Data Relationships

Customer → Request → Quote → Order

Order → Order Item → Furniture Item

Furniture Item → Category / Product Type

Order → Payment → Payment Allocation

This relational structure supports transaction tracking, inventory management, and financial records.

# Tools Used

Draw.io – Database conceptual modelling

Entity Relationship Diagram (ERD) methodology

Business rule analysis

