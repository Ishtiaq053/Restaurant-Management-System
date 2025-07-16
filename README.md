# Restaurant-Management-System
 Project Title:
Food Ordering System (Quetta Cafe Version)

 Project Objective:
To simulate a real-world restaurant order management system using Object-Oriented Programming and Data Structures like:
•	Arrays
•	Pointers
•	Queues/Stacks (likely behind placeOrder functions)
•	Binary Search Tree (for served orders, named root)
•	Dijkstra’s Algorithm (for delivery distance calculation)

 Major Functionalities
 1. Restaurant Setup
•	Name: Quetta Cafe
•	Address: Liberty Chowk, Lahore
•	Menu initialized with 10 dishes and their prices.
•	Menu and prices are stored dynamically using new string[11] and new int[11].

2. Main Menu Options
User can choose from:
Option	Functionality
1	View full food menu with prices
2	Place order (Take-Away, Delivery, Dine-In)
3	Serve an order (individually or all at once)
4	View pending orders
5	View or search served orders
6	Display total billing and earnings
0	Exit the program

 3. Order Placement Options
1. 🥡 Take-Away Customer
•	Takes name, age, quantity, dishIndex
•	Calculates bill = quantity * price
•	Calls placeOrderTakeAwayCustomer()

2. 🏠 Home Delivery Customer
•	Shows 5 delivery points (using Dijkstra’s Algorithm from index 0)
•	Calculates delivery charges = distance × 50 Rs
•	Total bill = food bill + delivery charges
•	Calls placeOrderHomeDeliveryCustomer()
________________________________________
3. 🍽️ Dine-In Customer
•	Similar to takeaway, but dine-in specific
•	Calls placeOrderDineInCustomer()

📦 4. Serving Orders
User can choose to:
•	Serve Take-Away
•	Serve Home Delivery
•	Serve Dine-In
•	Serve All at once
Each type likely uses a queue or stack internally.

📋 5. Pending Orders View
User can:
•	View pending orders of any type
•	View all pending orders

🧾 6. Served Orders
•	Stored using a BST (binary search tree) via a root node
•	User can:
o	Display all served orders
o	Search by name
o	Clear all served records

💰 7. Billing Info
•	Option 1: Show total pending order bill
•	Option 2: Show total earnings from served orders (using BST traversal and aggregation)

🧹 8. Cleanup
Before exit, the app:
•	Frees dynamic memory for menu and prices
•	Deletes all orders
•	Deletes BST of served customers

🔧 Data Structures and Concepts Used
Feature	Implementation
Dynamic memory for menu/price	new[] arrays
Graph Algorithm	dijkstra() used for delivery distance
Queues or Linked Lists	Likely used for pending orders
Binary Search Tree	For served order storage and retrieval
OOP	Classes like Restaurant, Customer, etc. (assumed from function names)

🧠 Potential Enhancements
•	Add admin authentication
•	Use file I/O for persistent order saving
•	Allow multiple dish orders per customer
•	Use class encapsulation for better design


