# FOOD ORDERING SYSTEM

## APPS INVOLVED
- There is a total of 3 apps which client.php, management.php and admin.php with 2 server-side which is server.php and restaurant.wsdl



## BRIEF EXPLANATION FOR EACH APPS

### Client.php:
**Purpose:** This application serves as a client interface to interact with the restaurant management system. It likely handles functionalities such as placing orders, viewing menus, and checking order status.

**Features:**
- Allows customers to view the menu (getMenu).
- Provides the ability to place orders (placeOrder).
- Checks the status of orders (getOrdersByStatus).
- Can cancel orders (cancelOrder).

### Management.php:

**Purpose:** This application is used by restaurant staff for day-to-day management tasks. It may include features for updating order statuses, viewing and managing orders, and possibly updating menu items.

**Features:**
- Manages orders (getOrdersByStatus, updateOrderStatus).
- Updates menu items (insertMenuItem, deleteMenuItem).
- Retrieves drink items (getDrinks).

### Admin.php:

**Purpose:** The admin application provides administrative functionalities for higher-level management. It typically includes features for managing users, viewing analytics or reports (like monthly sales), and possibly managing menu items or restaurant settings.

**Features:**
- Manages users and access permissions.
- Generates reports such as monthly sales (calculateMonthlySales).
- Accesses detailed analytics.



## URL ENDPOINTS
- http://localhost/restaurant/server.php
- http://localhost/restaurant/restaurant.wsdl 



## FUNCTIONS/FEATURES IN THE MIDDLEWARE

**Menu Management:**
- getMenu: Retrieves the restaurant's full menu.
- getDrinks: Retrieves specific drink items.
- insertMenuItem: Adds new menu items.
- deleteMenuItem: Removes menu items.

**Order Management:**
- placeOrder: Allows customers to place new orders.
- getOrdersByStatus: Retrieves orders based on their current status.
- updateOrderStatus: Updates the status of an existing order.
- cancelOrder: Cancels a pending order.

**Sales and Reporting:**
- calculateMonthlySales: Computes total sales for a specific month and year, aiding in financial reporting.

**User Management:**
- Ensures authentication and authorization mechanisms are in place to manage user roles and access levels.



## ARCHITECTURE DIAGRAM
1. client.php:

![Architec Diag DAD-Client php drawio](https://github.com/user-attachments/assets/55b1d60f-6fbb-4421-83b9-96323f4a780f)

2. management.php:

![Architec Diag DAD-Page-3 drawio](https://github.com/user-attachments/assets/005d011c-28a6-4275-8d9f-f295a060e362)

3. admin.php:

![Architec Diag DAD-Admin php drawio](https://github.com/user-attachments/assets/d40c9969-5d2e-49bb-9f8c-475473f6496d)



## DATABASE

**menu table:**
![image](https://github.com/user-attachments/assets/e80c8cd7-4048-4078-b298-a718c304c4fb)

**menu_drinks table:**
![image](https://github.com/user-attachments/assets/897d6040-e7ab-4856-b258-e1291623933d)


**orders table:**
![image](https://github.com/user-attachments/assets/5e72d6f4-d397-4bdd-83a9-6eb1f50353e7)


## VIDEO PRESENTATION LINK
- https://youtu.be/7L9OJMZpoeU

## HOW TO RUN?
1. Setup Database:
-    Use the provided SQL script(dbrestaurant.sql) to set up the database schema and initial data.

2. Configure PHP Server:
- Ensure the PHP server has access to the database and the correct configuration in (server.php).

3. Run Client Applications:
- Execute the the client.php, management.php and admin.php applications on different machines or environments as needed.

**IMPORTANT NOTES:**
- For PHP Server side, turn off the firewall.
- Change the URL IP address, insert the PHP Server Side IP address.
- You can you VSCODE to run this applications
