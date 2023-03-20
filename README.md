# sql-schema-template
This README explains the SQL schema used in this project and provides links to the corresponding SQL files in the project's GitHub repository.

## Overview
The SQL schema used in this project includes the following tables:

- `users`: stores information about the users of the system.
- `orders`: stores information about the orders placed by the users.
- `products`: stores information about the products available in the system.
- `order_items`: stores information about the items included in each order.

## SQL Files
The SQL schema is defined in the following files:

- [users.sql](./sql/tables/users.sql): defines the users table and its columns.
- [orders.sql](./sql/tables/orders.sql): defines the orders table and its columns. 
- [products.sql](./sql/tables/products.sql): defines the products table and its columns. 
- [order_items.sql](./sql/tables/order_items.sql): defines the order_items table and its columns. 

Each file contains the SQL code to create the corresponding table, along with any necessary constraints, such as primary keys or foreign keys.

## Explanation
### `users` table
The users table stores information about the users of the system. The table has the following columns:

`id`: unique identifier for each user.
`name`: name of the user.
`email`: email address of the user.
`password`: hashed password for the user's account.

### `orders` table
The orders table stores information about the orders placed by the users. The table has the following columns:

`id`: unique identifier for each order.
`user_id`: foreign key referencing the id column in the users table.
`order_date`: date the order was placed.
`total_price`: total price of the order.

### And so on..

We can extend by creating multiple folders such as 
```
.
├── README.md
└── sql
    ├── materialized_views
    │   └── sample.sql
    ├── queries
    │   └── sample.sql
    ├── tables
    │   └── sample.sql
    └── views
        └── sample.sql

6 directories, 5 files
```
