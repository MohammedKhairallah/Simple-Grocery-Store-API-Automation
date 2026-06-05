# Simple-Grocery-Store-API-Automation

This project tests the features of a grocery store website to make sure everything works perfectly.

---

## 📋 Project Scope
The test automation suite validates all core features of the grocery store application across multiple sections:
* **API Authentication:** Making sure users can register safely.
* **Store Status:** Monitors server health and operational availability.
* **Product Catalog:** Validates complete product search, structural queries, and item formatting.
* **Cart Management:** Manages full shopping cart Lifecycles (creating carts, adding items, updating quantities, and clearing items).
* **Order Processing:** Tests creating, modifying, reading, and completely deleting user orders.

---

## 🚀 Key Automation Logic

To make the tests run completely on their own without manual work, the project uses three smart steps:

* **Automatic Logins:** The project creates a user, grabs the secret access token, and automatically uses it to log into later steps.
* **Smart Data Sharing:** When a cart or an order is created, the project remembers its unique ID. It then automatically passes that ID to the next steps to view, change, or delete that specific item.
* **Error Checking:** The project intentionally sends wrong data (like broken IDs or missing logins) to make sure the website safely blocks them and shows the right error message.
---

## 📁 Repository Structure
* `/Screenshots` — Visual execution proofs and terminal validation run records.
* `Simple Grocery Store.postman_collection.json` — The complete executable suite containing all endpoint folders, pre-request automation logic, and test assertions.
* `Simple Grocery Store.postman_environment.json` — The isolated context configuration variables utilized across the execution runtime.

---

## 📊 How to Run This Project

Follow these simple steps to run the tests on your computer:

Open your terminal inside your project folder and execute this command to start the automation:
```bash
newman run "Simple Grocery Store.postman_collection.json" -e "Simple Grocery Store.postman_environment.json"
```
Or execute this command to create HTML also
```bash
newman run "Simple Grocery Store.postman_collection.json" -e "Simple Grocery Store.postman_environment.json" -r htmlextra
```

  
