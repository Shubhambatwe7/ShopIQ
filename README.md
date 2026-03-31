#  ShopIQ – Intelligent Dynamic Pricing E-Commerce Platform

## Overview

ShopIQ is a dynamic e-commerce platform that automatically adjusts product prices based on real-time demand, user behavior, and customer feedback. The system enhances customer experience while optimizing pricing strategies for sellers.

---

## Objectives

* Implement real-time dynamic pricing
* Improve customer engagement and transparency
* Optimize sales and inventory management
* Build a scalable and responsive e-commerce platform

---

##  System Architecture

ShopIQ follows a **3-tier architecture**:

### 1. Frontend Layer

* Built using HTML and CSS
* Provides interface for browsing, purchasing, and reviewing products

### 2. Backend Layer

* Node.js (Express.js) + PHP
* Handles APIs, authentication, and pricing logic

### 3. Database Layer

* MySQL
* Stores users, products, reviews, and pricing data

---

## Installation & Setup Guide

###  Prerequisites

Ensure the following are installed:

* Node.js (v16 or higher)
* PHP (v7 or higher)
* MySQL Server
* Git
* VS Code (recommended)

---

###  Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/shopiq.git
cd shopiq
```

---

###  Step 2: Database Setup

1. Start MySQL server
2. Create database:

```sql
CREATE DATABASE shopiq;
USE shopiq;
```

3. Import schema:

```bash
mysql -u root -p shopiq < database/schema.sql
```

---

### 🔌 Step 3: Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file:

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=shopiq
```

Start backend server:

```bash
npm start
```

---

###  Step 4: PHP Server (if applicable)

```bash
cd backend/php
php -S localhost:8000
```

---

###  Step 5: Run Frontend

* Open `frontend/index.html`
  OR
* Use VS Code Live Server

---

### Step 6: Access Application

| Service     | URL                                 |
| ----------- | ----------------------------------- |
| Frontend    | http://localhost:3000 or index.html |
| Backend API | http://localhost:5000               |
| PHP Server  | http://localhost:8000               |

---

##  Working of the Project

ShopIQ operates using a **data-driven dynamic pricing mechanism** that continuously adapts product prices based on user activity and demand patterns.

###  Detailed Workflow

#### 1. User Interaction Layer

* Users register/login into the platform
* Browse products, view details, and add items to cart
* Submit ratings and reviews

#### 2. Data Collection Layer

The system continuously captures user activity such as:

* Product views
* Search frequency
* Cart additions
* Purchase history
* Ratings and reviews

This data acts as the foundation for price decision-making.

#### 3. Dynamic Pricing Engine (Core Module)

* The pricing algorithm analyzes collected data in real-time
* It evaluates demand trends and user sentiment

Price adjustment logic:

*  High demand → Price increases
*  Low demand → Price decreases
*  Positive reviews → Price may increase
*  Negative reviews → Price may decrease

This ensures "optimal and competitive pricing" at all times.

#### 4. Backend Processing

* Node.js and PHP handle business logic
* APIs process requests from frontend
* Pricing algorithm is executed on the server side

#### 5. Database Operations

* MySQL stores:

  * User data
  * Product details
  * Reviews
  * Updated pricing
* Historical pricing data is maintained for analysis

#### 6. Real-Time Price Update

* Updated prices are sent back to the frontend
* Users see the latest price dynamically
* Ensures transparency and responsiveness

#### 7. Decision & Feedback Loop

* Users make purchase decisions based on updated prices
* Their behavior again feeds into the system
* This creates a **continuous feedback loop** improving pricing accuracy over time

---

##  Key Features

* Dynamic pricing algorithm
* Real-time demand tracking
* User authentication system
* Review and rating system
* Responsive UI

---

##  Testing

* **Unit Testing:** Pricing algorithm validation
* **Integration Testing:** API and database communication
* **Manual Testing:** User interface and workflows

---

##  Troubleshooting

| Issue                     | Solution                 |
| ------------------------- | ------------------------ |
| Database connection error | Check `.env` credentials |
| Server not starting       | Run `npm install`        |
| Port already in use       | Change PORT              |
| PHP server error          | Verify PHP installation  |

---

##  Scalability & Performance

* Supports up to **10,000 concurrent users**
* Modular backend architecture
* Optimized database queries

---

## Future Enhancements

* AI-based demand prediction
* Personalized pricing
* Payment gateway integration
* Admin analytics dashboard


##  License

This project is developed for academic purposes.

---

##  Conclusion

ShopIQ showcases how real-time data and intelligent algorithms can transform traditional e-commerce systems into adaptive, efficient, and user-centric platforms.
