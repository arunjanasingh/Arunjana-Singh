# Problem Statement & Project Scope

## 1. Problem Statement
Small and medium-sized retail shopkeepers often struggle with manual billing processes, stock tracking inaccuracies, and complex discount calculations. Manual billing slows down customer checkouts, increases the risk of human error in pricing or discounts, and makes real-time inventory updates difficult to maintain without dedicated software solutions.

## 2. Scope of the Project
The **Shop Bill Calculator** is a lightweight desktop application designed to streamline retail point-of-sale operations. 

### In-Scope:
* Automated bill generation based on item codes and stock quantities.
* Tiered subtotal discount logic and validation for membership discounts.
* Admin panel for managing inventory (adding new products and restocking).
* Real-time stock updates upon item selection during billing.

### Out-of-Scope:
* Multi-store cloud synchronization.
* Payment gateway integration (credit cards/UPI).

## 3. Target Users
* **Retail Shopkeepers & Cashiers:** Primary users who operate the billing interface to create customer receipts quickly.
* **Store Administrators & Owners:** Users who access the admin panel using secure credentials to monitor and update inventory levels.
* **Retail Customers:** End beneficiaries receiving itemized bills with applied discounts.

## 4. High-Level Features
* **Interactive GUI:** User-friendly Tkinter-based interface for navigation between billing and administrative features.
* **Smart Discount Processing:** 
  * *Subtotal Tiered Discounts:* 5% for $\ge ₹100$, 10% for $\ge ₹200$, and 20% for $\ge ₹500$.
  * *Membership Benefits:* Additional 10% discount for registered members verified via regex matching (name + 10-digit phone number).
* **Inventory Management:** Administrative controls to view stock status, adjust current stock, and append new inventory items.
* **Input Validation & Error Handling:** Safeguards against invalid item codes, non-numeric quantity inputs, and out-of-stock items.
