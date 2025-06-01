# 🛒 Online Shopping System - Java OOP Project

This project simulates a simple Online Shopping System using Java and object-oriented programming (OOP) principles. It includes user accounts, customers, products, shopping carts, orders, and payments.

## 🚀 Features

- User login simulation (`WebUser`)
- Customer account management
- Product catalog
- Shopping cart with line items
- Order creation and status tracking
- Payment handling

---

## 🧱 Class Overview

### 🔐 `WebUser`
Represents a web user with:
- `loginId`, `password`, `email`

### 👤 `Customer`
Models a customer with:
- `id`, `billingAddress`, `openDate`, `isClosed`

### 🧾 `Account`
(Structurally similar to Customer, could be integrated further)

### 📦 `Product`
Represents a product with:
- `id`, `name`, `supplier`

### 🛒 `ShoppingCart`
- Stores list of `LineItem`s (product + quantity + price)
- `createdDate`, `addItem(LineItem item)`

### 📋 `LineItem`
- Contains a `Product`, quantity, and price

### 📑 `Order`
- Contains order `number`, `orderedDate`, `shipToDate`, `total`, `status` (`OrderStatus` enum)

### 💰 `Payment`
- Tracks payment `id`, `paidDate`, `total`

### 🚚 `OrderStatus` (Enum)
- States: `NEW`, `PROCESSING`, `SHIPPED`, `DELIVERED`, `CANCELLED`

---

## 💡 OOP Concepts Demonstrated

- **Encapsulation**: Private fields with constructors
- **Abstraction**: Separation of user, cart, order, and payment responsibilities
- **Enum usage**: Clear and manageable order states
- **Object Interaction**: Objects collaborate to simulate shopping flow

---

## 💻 How to Run

### 🧰 Requirements
- Java JDK 8 or above
- Terminal or IDE (e.g., IntelliJ, Eclipse)

### ▶️ Steps
1. Save the file as `OnlineShoppingSystem.java`
2. Compile and run:

```bash
javac OnlineShoppingSystem.java
java OnlineShoppingSystem
