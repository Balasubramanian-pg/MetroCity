### **Project Data Asset Overview**

The "MetroCity" end-to-end project integrates both structured and unstructured data to provide a comprehensive 360-degree view of the business. These assets are ingested into the Bronze layer, refined in the Silver layer, and aggregated for business intelligence in the Gold layer.

---

### **1. Structured Data**

This category represents the core transactional and master data of the retail business, typically originating from an OLTP (Online Transaction Processing) database.

| Data Asset | Source File | Description | Key Attributes | Role in the Project |
| :--- | :--- | :--- | :--- | :--- |
| **Customer Data** | `customers.csv` | Contains demographic and contact information for each registered customer. This serves as the customer dimension table. | `CustomerID`, `CustomerName`, `Email`, `Location`, `SignupDate` | Used to analyze customer behavior, identify top customers by sales, and segment customers by location or tenure. |
| **Product Data** | `products.csv` | A master list of all products available for sale, including their classification and inventory details. This is the product dimension table. | `ProductID`, `ProductName`, `Category` (e.g., Fashion, Electronics), `StockQuantity`, `UnitPrice` | Essential for inventory management, sales analysis by product category, and identifying top-selling or low-stock products. |
| **Transactional Data (Orders)** | `orders.csv` | The primary fact table, recording every sales transaction that has occurred. It links customers to the products they purchased. | `OrderID`, `OrderDate`, `CustomerID`, `ProductID`, `QuantitySold`, `TotalAmount`, `PaymentMethod` | Forms the foundation for all core sales KPIs, including total revenue, sales trends over time, and calculating customer lifetime value. |
