# BikeSystemSQL

A collection of T-SQL scripts defining relational database schemas. The repository contains two separate schemas: a bike shop sales/inventory schema (brands, categories, products, customers, staff, stores, stock, and orders) and a restaurant management schema (restaurants, tables, and menu items with orders).

## Features

**Bike Shop Schema**
- **Brands** and **Categories** for classifying products
- **Products** (name, brand, category, model year, list price)
- **Customers** (contact and address details)
- **Staffs** (linked to a store, with an optional manager)
- **Stores** (contact and address details)
- **Stocks** (product quantity per store)
- **Orders** and **Order_items** (order status, dates, linked customer/store/staff, line items with quantity, price, and discount)

**Restaurant Schema**
- **Restaurants** (name, branch code, total orders, total revenue, active tables)
- **Tables** (table number, capacity, linked restaurant, order count)
- **MenuItems** (name, price, category, linked restaurant, total sold)
- **OrderItems** (order, menu item, quantity, price)

## Technologies

- T-SQL (Transact-SQL)
- Microsoft SQL Server

## Requirements

- Microsoft SQL Server (or SQL Server Express / LocalDB)
- SQL Server Management Studio (SSMS) or Azure Data Studio to run the scripts

## Installation and Run

git clone https://github.com/RenaMehdiyeva88/BikeSystemSQL.git
cd BikeSystemSQL

Create a database in SQL Server (or update the `USE [...]` line in each script to match your own database name), then run the scripts. Note: the repository holds two independent schemas — decide which one you need and run only the related scripts, in an order that respects foreign key dependencies, for example:

**Bike shop schema:**
- dbo.Brands.Table.sql
- dbo.Categories.Table.sql
- dbo.Products.Table.sql
- dbo.Customers.Table.sql
- dbo.Stores.Table.sql
- dbo.Staffs.Table.sql
- dbo.Stocks.Table.sql
- dbo.Orders.Table.sql
- dbo.Order_items.Table.sql

**Restaurant schema:**
- dbo.Restaurants.Table.sql
- dbo.Tables.Table.sql
- dbo.MenuItems.Table.sql
- dbo.OrderItems.Table.sql

## Project Structure

BikeSystemSQL/
├── dbo.Brands.Table.sql
├── dbo.Categories.Table.sql
├── dbo.Products.Table.sql
├── dbo.Customers.Table.sql
├── dbo.Stores.Table.sql
├── dbo.Staffs.Table.sql
├── dbo.Stocks.Table.sql
├── dbo.Orders.Table.sql
├── dbo.Order_items.Table.sql
├── dbo.Restaurants.Table.sql
├── dbo.Tables.Table.sql
├── dbo.MenuItems.Table.sql
├── dbo.OrderItems.Table.sql
└── README.md

## Author

RenaMehdiyeva88 (https://github.com/RenaMehdiyeva88)
