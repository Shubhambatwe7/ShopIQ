# 🛒 ShopIQ – Dynamic E-Commerce Platform

ShopIQ is an intelligent e-commerce platform that dynamically adjusts product prices based on real-time demand, user behavior, and market trends. The goal is to provide fair pricing for customers while optimizing revenue for sellers.

---

## Features

-  User Authentication (Login/Register)
-  Product Management System
-  Review & Rating System
-  Cart & Wishlist Functionality
-  Dynamic Pricing Engine (based on demand & reviews)
-  Real-time price updates
-  Responsive UI (Desktop & Mobile)

---

## Tech Stack

**Frontend:**
- HTML
- CSS

**Backend:**
- Node.js (Express.js)
- PHP

**Database:**
- MySQL

---

##  Setup Instructions

Follow these steps to set up and run the project locally.

---

### Prerequisites

Make sure you have installed:

- Node.js (v16+)
- PHP (v7+)
- MySQL
- Git
- A code editor (VS Code recommended)

---
##  Working of ShopIQ

###  Step-by-Step Workflow

1. **User Interaction**
   - Users register/login and browse products.
   - They can view details, add items to cart, and leave reviews/ratings.

2. **Data Collection**
   - The system continuously tracks:
     - Product views
     - Purchase frequency
     - User ratings and reviews
     - Cart additions

3. **Dynamic Pricing Engine**
   - A pricing algorithm processes collected data.
   - Price updates are based on:
     -  High demand → Price increases  
     -  Low demand → Price decreases  
     -  Better ratings → Price may increase  
     -  Poor feedback → Price may drop  

4. **Backend Processing**
   - The backend (Node.js + PHP) handles:
     - API requests
     - Business logic
     - Communication with the database

5. **Database Management**
   - MySQL stores:
     - User data
     - Product details
     - Reviews and ratings
     - Pricing history

6. **Real-Time Updates**
   - Updated prices are fetched and displayed on the frontend.
   - Users always see the latest price without manual refresh (if implemented with live updates).

7. **User Experience**
   - Smooth UI allows users to:
     - Shop efficiently
     - Compare dynamic prices
     - Make informed decisions

### Clone the Repository

```bash
git clone https://github.com/your-username/shopiq.git
cd shopiq
