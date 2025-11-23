# 🧹 Cleaning a PostgreSQL Database

## Clean PostgreSQL Database

In this project, we will work with data from a **hypothetical Super Store** to challenge and enhance our **SQL skills in data cleaning**.  
This project will involve:

- Identifying **top categories** based on the highest profit margins  
- Detecting **missing values**  
- Applying comprehensive SQL concepts in a **practical scenario**

---

## 📚 Data Dictionary

### **orders**

| Column      | Definition                                         | Data type         | Comments                                                  |
|-------------|-----------------------------------------------------|-------------------|-----------------------------------------------------------|
| row_id      | Unique Record ID                                    | INTEGER           |                                                           |
| order_id    | Identifier for each order in table                  | TEXT              | Connects to `order_id` in `returned_orders` table         |
| order_date  | Date when order was placed                          | TEXT              |                                                           |
| market      | Market order_id belongs to                          | TEXT              |                                                           |
| region      | Region Customer belongs to                          | TEXT              | Connects to `region` in `people` table                    |
| product_id  | Identifier of Product bought                        | TEXT              | Connects to `product_id` in `products` table              |
| sales       | Total Sales Amount for the Line Item                | DOUBLE PRECISION  |                                                           |
| quantity    | Total Quantity for the Line Item                    | DOUBLE PRECISION  |                                                           |
| discount    | Discount applied for the Line Item                  | DOUBLE PRECISION  |                                                           |
| profit      | Total Profit earned on the Line Item                | DOUBLE PRECISION  |                                                           |

---

### **returned_orders**

| Column    | Definition                                          | Data type |
|-----------|------------------------------------------------------|-----------|
| returned  | Yes values for Order / Line Item Returned            | TEXT      |
| order_id  | Identifier for each order in table                   | TEXT      |
| market    | Market order_id belongs to                           | TEXT      |

---

### **people**

| Column  | Definition                                        | Data type |
|---------|----------------------------------------------------|-----------|
| person  | Name of Salesperson credited with Order           | TEXT      |
| region  | Region Salesperson is operating in                | TEXT      |

---

### **products**

| Column        | Definition                                         | Data type |
|---------------|-----------------------------------------------------|-----------|
| product_id    | Unique Identifier for the Product                   | TEXT      |
| category      | Category Product belongs to                         | TEXT      |
| sub_category  | Sub Category Product belongs to                     | TEXT      |
| product_name  | Detailed Name of the Product                        | TEXT      |

---

![Super Store ERD](SuperStore_ERD.png)
