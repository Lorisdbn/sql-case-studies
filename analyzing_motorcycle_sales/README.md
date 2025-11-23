![Motorcycle](motorcycle.jpg)

## 🏍️ Motorcycle Parts Sales Analysis

We're working for a company that sells **motorcycle parts**, and they’ve asked for help analyzing their **sales data**.

The company operates **three warehouses** in the region, selling to both **retail and wholesale** clients. They offer a range of products and accept **credit card**, **cash**, and **bank transfer** as payment methods. However, each payment type incurs a **different fee**.

---

## 🎯 Objective

The **Board of Directors** wants to better understand:

- **Wholesale revenue** by product line
- How revenue varies **month-to-month**
- How revenue differs **across warehouses**

You’ve been tasked with:

✅ Calculating **net revenue** for each product line  
✅ Grouping results by **month** and **warehouse**  
✅ **Filtering** for **Wholesale** orders only

---

## 🗃️ Available Data: `sales` Table

| Column        | Data Type | Description                                                                 |
|---------------|-----------|-----------------------------------------------------------------------------|
| order_number  | VARCHAR   | Unique order number                                                         |
| date          | DATE      | Date of the order (from June to August 2021)                                |
| warehouse     | VARCHAR   | Warehouse where the order was made — North, Central, or West                |
| client_type   | VARCHAR   | Either "Retail" or "Wholesale"                                              |
| product_line  | VARCHAR   | Type of product ordered                                                     |
| quantity      | INT       | Number of products ordered                                                  |
| unit_price    | FLOAT     | Price per product (in dollars)                                              |
| total         | FLOAT     | Total price of the order (in dollars)                                       |
| payment       | VARCHAR   | Payment method — Credit card, Transfer, or Cash                             |
| payment_fee   | FLOAT     | Percentage fee applied to total, depending on the payment method            |

> 🧮 **Note:** Net revenue = `total - (total * payment_fee / 100)`

---

## 📤 Expected Output Format

The final query should return a table like this:

| product_line  | month | warehouse | net_revenue |
|---------------|-------|-----------|-------------|
| product_one   | ---   | ---       | ---         |
| product_one   | ---   | ---       | ---         |
| product_one   | ---   | ---       | ---         |
| product_one   | ---   | ---       | ---         |
| product_two   | ---   | ---       | ---         |
| ...           | ...   | ...       | ...         |
