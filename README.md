# 🍔 Starbites Food Ordering System

A complete web-based food ordering and management system developed for Starbites restaurant as a field trip project.

## 📋 Overview

This system automates the food ordering process at Starbites, addressing challenges such as manual order processing, delays during peak hours, and difficulty maintaining accurate records.

## ✨ Features

### Customer Features
- **Interactive Menu Display** - Browse available food items with prices
- **Real-time Cart Management** - Add/remove items and adjust quantities
- **Order Placement** - Submit orders with delivery details
- **Order Confirmation** - Receive instant order confirmation with order ID

### Admin Features
- **Order Management Dashboard** - View and manage all customer orders
- **Status Updates** - Change order status (Pending → Processing → Completed)
- **Real-time Statistics** - Monitor total orders, pending orders, and revenue
- **Order History** - Access complete order records

### Reports Features
- **Daily Sales Reports** - View today's orders and revenue
- **Popular Items Tracking** - Identify most ordered menu items
- **Revenue Analytics** - Track sales performance

## 🛠️ Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript (ES6)
- **Backend**: PHP 7.4+
- **Database**: MySQL 5.7+
- **Design**: Custom CSS with gradient backgrounds and animations

## 📂 Project Structure

```
starbites-system/
│
├── index.html              # Main application interface
├── styles.css              # Styling and responsive design
├── script.js               # Client-side functionality
├── config.php              # Database configuration
├── database.sql            # Database schema
├── process_order.php       # Order processing backend
├── get_orders.php          # Retrieve orders API
├── update_order.php        # Update order status API
├── reports.php             # Generate reports API
└── README.md               # This file
```

## 🚀 Installation

### Prerequisites
- XAMPP, WAMP, or LAMP (Apache + MySQL + PHP)
- Web browser (Chrome, Firefox, Safari, Edge)

### Setup Instructions

1. **Install Web Server**
   - Download and install XAMPP from https://www.apachefriends.org
   - Start Apache and MySQL services

2. **Create Database**
   ```sql
   - Open phpMyAdmin (http://localhost/phpmyadmin)
   - Create database: starbites_db
   - Import database.sql file
   ```

3. **Configure Database Connection**
   - Open `config.php`
   - Update credentials if needed:
   ```php
   define('DB_HOST', 'localhost');
   define('DB_USER', 'root');
   define('DB_PASS', '');
   define('DB_NAME', 'starbites_db');
   ```

4. **Deploy Files**
   - Copy all files to: `C:\xampp\htdocs\starbites\`
   - Or your web server's root directory

5. **Access System**
   - Open browser
   - Navigate to: `http://localhost/starbites/`

## 📱 How to Use

### For Customers

1. **Browse Menu**
   - View available food items on the homepage
   - Each item shows name, price, and emoji icon

2. **Add Items to Cart**
   - Click on desired menu items
   - Use +/- buttons to adjust quantities
   - View cart summary at bottom

3. **Place Order**
   - Fill in customer details (Name, Phone, Address)
   - Click "Place Order" button
   - Receive order confirmation

### For Administrators

1. **Access Admin Dashboard**
   - Click "Admin Dashboard" tab
   - View all orders and statistics

2. **Manage Orders**
   - View order details in table format
   - Update order status using dropdown menus
   - Monitor pending orders

3. **View Reports**
   - Click "Reports" tab
   - Check daily sales statistics
   - See most popular items

## 🎯 System Benefits

- ✅ **Faster Service** - Automated order processing reduces wait times
- ✅ **Reduced Errors** - Digital orders eliminate mix-ups
- ✅ **Better Records** - Secure database storage of all transactions
- ✅ **Improved Efficiency** - Real-time order tracking and status updates
- ✅ **Data Analytics** - Sales reports for better decision making

## 🔒 Security Features

- **SQL Injection Prevention** - Prepared statements and input sanitization
- **XSS Protection** - HTML special characters encoding
- **Data Validation** - Server-side input validation
- **Transaction Management** - Database transactions for data integrity

## 📊 Database Schema

### Tables

**orders** - Main orders table
- order_id (Primary Key)
- customer_name
- customer_phone
- delivery_address
- total_amount
- order_status
- order_date

**order_items** - Order line items
- item_id (Primary Key)
- order_id (Foreign Key)
- food_item
- quantity
- unit_price
- subtotal

**menu_items** - Food menu catalog
- menu_id (Primary Key)
- item_name
- item_price
- item_category
- is_available

## 🔮 Future Enhancements

- User authentication and login system
- SMS/Email order notifications
- Payment gateway integration
- Customer loyalty program
- Mobile application (iOS/Android)
- Real-time order tracking with GPS
- Multi-branch support
- Online payment processing

## 👨‍💻 Developer Information

**Name**: Abdul-Mumin Mahafuz  
**Index Number**: 1696791203  
**Institution**: Ghana Communication Technology University  
**Department**: Computer Science  
**Course**: Field Trip and Report Writing  
**Lecturer**: Dr. Martin Mabeifam Ujakpa  
**Year**: 2025

## 📝 Project Context

This system was developed as part of a field trip to Starbites restaurant, where manual order processing was identified as a major challenge. The proposed solution addresses:

- Order mix-ups during busy periods
- Delays in order processing
- Difficulty maintaining accurate records
- Lack of customer order history

## 🐛 Troubleshooting

### Database Connection Error
```
Solution: 
- Check if MySQL is running
- Verify credentials in config.php
- Ensure database exists
```

### Page Not Loading
```
Solution:
- Verify Apache is running
- Check file permissions
- Clear browser cache
```

### Orders Not Saving
```
Solution:
- Check PHP error logs
- Verify database tables exist
- Test database connection
```

## 📞 Support

For issues or questions:
- Check the troubleshooting section
- Review PHP error logs
- Verify database connection settings

## 📄 License

This project is an educational assignment for Ghana Communication Technology University.

## 🙏 Acknowledgments

- **Starbites Management** - For allowing the field visit
- **Dr. Martin Mabeifam Ujakpa** - For guidance and supervision
- **GCTU Computer Science Department** - For academic support

---

**Version**: 1.0.0  
**Last Updated**: December 2025  
**Status**: Active Development

## 🌟 Live Demo

[Add your hosted link here after deployment]

## 📸 Screenshots

[Add screenshots of the system here]

---

© 2025 Abdul-Mumin Mahafuz | Ghana Communication Technology University