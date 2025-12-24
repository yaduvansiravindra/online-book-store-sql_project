📚 Online Book Store – SQL Database Project
Project Overview
This is a real-world SQL database project for an Online Book Store.
It manages book inventory, customer records, and orders. The system is designed to handle day-to-day bookstore operations such as tracking available stock, recording purchases, and analyzing sales.

Database Schema
Books Table
Stores all book details.
- Book_ID (PK)
- Title
- Author
- Genre
- Published_Year
- Price
- Stock
Customers Table
Stores customer information.
- Customer_ID (PK)
- Name
- Email
- Phone
- City
- Country
Orders Table
Stores purchase records.
- Order_ID (PK)
- Customer_ID (FK → Customers.Customer_ID)
- Book_ID (FK → Books.Book_ID)
- Order_Date
- Quantity
- Total_Amount

ER Diagram
+-----------+           +-------------+           +--------+
| Customers |           |   Orders    |           | Books  |
+-----------+           +-------------+           +--------+
| Customer_ID|<-------> | Customer_ID |           | Book_ID|
| Name       |           | Order_ID    | <------->| Title  |
| Email      |           | Book_ID     |           | Author |
| Phone      |           | Order_Date  |           | Genre  |
| City       |           | Quantity    |           | Year   |
| Country    |           | Total_Amount|           | Price  |
+-----------+           +-------------+           | Stock  |
                                                  +--------+



Data Import
CSV files are used to load data into tables:
- Books.csv → Books table
- Customers.csv → Customers table
- Orders.csv → Orders table

Key Features
- 📖 Inventory Management: Track available stock of books.
- 👤 Customer Records: Store customer details for communication and analysis.
- 🛒 Order Processing: Record purchases with quantity and total amount.
- 💰 Revenue Tracking: Calculate total revenue from all orders.
- 📊 Sales Insights: Identify top-selling genres, authors, and customers.
- 🌍 Customer Analytics: Find customer distribution by city/country.
- 📦 Stock Monitoring: Check remaining stock after fulfilling orders.

Example Use Cases
- Store Manager can check which books are low in stock.
- Sales Team can identify top customers and regions generating revenue.
- Analytics Team can calculate total revenue and genre-wise sales.
- Admin can import new books/customers/orders via CSV files.

Business Value
- Helps bookstore owners manage inventory efficiently.
- Provides insights into customer behavior and sales trends.
- Supports decision-making for restocking and marketing.
- Demonstrates SQL skills in a real-world business scenario.
