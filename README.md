# 🛒 Order Management System - Web Frontend (AAD Task 01)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

A modern, responsive, single-page-feel web client for the **Order Management System** developed as part of **AAD Task 01**. Built using pure HTML5, modern CSS3 styling, JavaScript (ES6+), and jQuery AJAX for seamless RESTful API communication with JWT authentication support.

---

## 🌟 Key Features

- 🔐 **JWT User Authentication**: Secure Login & Registration system with automated JWT token handling and LocalStorage persistence.
- 📊 **Real-time Dashboard**: Interactive dashboard displaying live metric cards for Total Customers, Total Stock Items, and Total Orders.
- 👥 **Customer Management**: Complete CRUD functionality (Save, Update, Delete, Search by ID, and Refreshable Data Table).
- 📦 **Item & Inventory Management**: Manage inventory stock quantities (`itemQTY`), unit pricing (`itemPrice`), and item profiles.
- 🛒 **Order Processing & Placement**: Dynamic cart placement supporting multi-item orders, automated real-time price calculations, customer verification, and order history tracking.
- 🎨 **Modern Glassmorphic UI**: Ultra-clean UI featuring CSS custom properties, smooth hover micro-animations, mobile responsiveness, and intuitive navigation.

---

## 🛠️ Technology Stack

| Layer | Technology | Details |
| :--- | :--- | :--- |
| **Markup** | HTML5 | Semantic structural elements for accessibility & performance |
| **Styling** | Custom CSS3 | Modern Design Tokens, Responsive Flexbox & Grid layouts |
| **Scripting & DOM** | JavaScript (ES6+) & jQuery 3.6 | Asynchronous DOM manipulation & Event handling |
| **API Integration** | jQuery AJAX (`$.ajax`) | Asynchronous HTTP requests with Bearer JWT Authorization headers |
| **Data Storage** | Browser `localStorage` | Persisting JWT Access Tokens and User Session metadata |

---

## 📁 Repository Structure

```text
AAD Task 01 Frontend/
├── 📄 Login.html       # User authentication & sign-in page
├── 📄 Signup.html      # New user registration page
├── 📄 Dashboard.html   # System metrics overview & quick action shortcuts
├── 📄 Customer.html    # Customer profile CRUD operations & listings
├── 📄 Item.html        # Product & stock management console
├── 📄 Order.html       # Interactive checkout, cart management & order logs
├── 🎨 Style.css        # Centralized UI Design System & Component Styles
└── 📘 README.md        # Project documentation & integration guide
```

---

## 🔗 Backend REST API Integration

The frontend seamlessly connects to the Spring Boot REST API running on `http://localhost:8080`.

### 🔑 Auth Endpoints
- **POST** `/api/users/login` - Authenticate user & receive JWT token.
- **POST** `/api/users/save` - Register a new user account.

### 👤 Customer Endpoints
- **GET** `/api/customers/all` - Fetch all customers.
- **POST** `/api/customers/save` - Create a new customer profile.
- **PUT** `/api/customers/update` - Update an existing customer record.
- **DELETE** `/api/customers/delete/{id}` - Remove customer by ID.
- **GET** `/api/customers/search/{id}` - Search customer details by ID.

### 📦 Item Endpoints
- **GET** `/api/items/all` - Fetch all items in inventory.
- **POST** `/api/items/save` - Add new product item.
- **PUT** `/api/items/update` - Modify item details, stock quantity, or unit price.
- **DELETE** `/api/items/delete/{id}` - Remove item by ID.
- **GET** `/api/items/search/{id}` - Query item by ID.

### 🛒 Order Endpoints
- **POST** `/api/orders/save` - Place new order with customer and list of items.
- **GET** `/api/orders/all` - Retrieve complete order history.

---

## 🚀 Getting Started

### Prerequisites

1. A modern Web Browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Brave).
2. The **Order Management System Backend API** running on `http://localhost:8080`.

### 📦 Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/chathunga2007/ITS1114-Order-Management-System-AAD-Task-01-Frontend.git
   ```

2. **Navigate into Project Directory**:
   ```bash
   cd ITS1114-Order-Management-System-AAD-Task-01-Frontend
   ```

3. **Run the Frontend**:
   - Open `Login.html` in your web browser, **OR**
   - Use VS Code **Live Server** extension to launch the app locally.

---

## 💻 Workflow Guide

1. **Login / Register**: Access `Login.html` or `Signup.html` to authenticate.
2. **Dashboard Overview**: After successful login, you will be redirected to `Dashboard.html` with real-time statistics.
3. **Manage Customers**: Go to `Customer.html` to create or edit customer profiles.
4. **Manage Stock**: Go to `Item.html` to add inventory and manage product prices.
5. **Place Orders**: Go to `Order.html` to enter customer ID, select items, view cart total, and place orders.

---

## 👨‍💻 Author

<div align="center">
  Developed with ❤️ by **Chathunga Bimsara** for **ITS1114 / AAD Task 01** &nbsp;|&nbsp; IJSE Task 01 Project Frontend
</div>
- **GitHub**: [@chathunga2007](https://github.com/chathunga2007)