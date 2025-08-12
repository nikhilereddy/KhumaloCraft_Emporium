# KhumaloCraft_Emporium
KhumaloCraft Emporium is an ASP.NET Core MVC web app integrated with an Azure SQL database. It enables dynamic product management, user registrations, and order processing. Clients can browse crafts, place orders, and view history, while admins manage products and process client orders efficiently in real time.

# KhumaloCraft Emporium Web Application — POE Part 2

## Overview
KhumaloCraft Emporium is an ASP.NET Core MVC web application that manages craft products, customers, and transactions. This Part 2 of the Portfolio of Evidence (POE) enhances the initial app by integrating a SQL Server database deployed on Azure. The application now supports dynamic product management, client ordering, and order processing.

---

## Table of Contents
- [Project Description](#project-description)  
- [Features](#features)  
- [Technologies Used](#technologies-used)  
- [Database Design](#database-design)  
- [Deployment](#deployment)  
- [Usage](#usage)  
- [Setup and Run](#setup-and-run)  
- [Links](#links)  
- [Future Enhancements](#future-enhancements)  
- [Author](#author)  

---

## Project Description
This project integrates a SQL Server database with the KhumaloCraft Emporium web app, enabling storage and retrieval of user, product, and order data. The database is hosted on Azure SQL Database and connected seamlessly to the web application, allowing real-time transactions and data management by users and admins.

---

## Features
- SQL Server database design for users, products, and orders  
- Azure deployment of the SQL database and web app  
- Dynamic product listing on the **My Work** page  
- Admin interface for adding new products  
- Clients can place orders and view order history  
- Admins can view and process client orders  

---

## Technologies Used
- ASP.NET Core MVC  
- C#  
- SQL Server  
- Azure SQL Database  
- Entity Framework Core  
- HTML, CSS, JavaScript  

---

## Database Design
The database schema contains the following core tables:

- **Users**: Stores user profiles, login credentials, and roles.  
- **Products**: Stores product details such as name, price, category, and availability.  
- **Orders**: Stores orders placed by clients, linking users with products and tracking order status.

---

## Deployment
- Database deployed on Azure SQL Database service  
- Web application deployed on Azure App Service  
- Connection strings configured for Azure SQL connectivity in appsettings.json  

---

## Usage
1. Access the deployed web application via the provided URL.  
2. View products dynamically loaded from the Azure SQL database on the **My Work** page.  
3. Admin users can add new products through the product management interface.  
4. Clients can browse products, place orders, and view their previous orders.  
5. Admins can view and manage all client orders.

---

## Setup and Run

```bash
# Clone the repository
git clone https://github.com/yourusername/KhumaloCraftEmporium.git
cd KhumaloCraftEmporium

# Restore dependencies
dotnet restore

# Update connection string in appsettings.json
# Example:
# "ConnectionStrings": {
#   "DefaultConnection": "Server=tcp:yourserver.database.windows.net,1433;Initial Catalog=yourdb;Persist Security Info=False;User ID=youruser;Password=yourpassword;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection Timeout=30;"
# }

# Apply migrations and update the database (if using EF Core migrations)
dotnet ef database update

# Run the application
dotnet run

# The application will be available at https://localhost:5001 or similar
Links
Deployed Application: https://yourapp.azurewebsites.net

GitHub Repository: https://github.com/nikhilereddy/KhumaloCraft_Emporium

Future Enhancements
Implement advanced authentication and role-based authorization

Integrate payment gateway for order processing

Improve UI/UX with responsive and mobile-friendly design

Add email notifications for order confirmations and status updates

Author
Nikhile Reddy


