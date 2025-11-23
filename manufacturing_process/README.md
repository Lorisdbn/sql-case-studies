# ⚙️ Manufacturing processes & statistical process control (SPC)

![Manufacturing Process](manufacturing.jpg)

Manufacturing processes for any product are like putting together a puzzle.  
Products are assembled **step by step**, and keeping a **close eye** on the process is crucial.

---

## 🎯 Project Context

In this project, we're supporting a team that wants to **improve how they monitor and control a manufacturing process**.  
The goal is to implement a **methodical approach** known as **Statistical Process Control (SPC)**.  

SPC is a well-established strategy that uses **data** to determine whether the process is working properly.  
Processes are only adjusted if measurements fall **outside of an acceptable range**.

---

## 📐 Control Limits

This acceptable range is defined by:

- **Upper Control Limit (UCL)**  
- **Lower Control Limit (LCL)**  

The formulas for these control limits are applied to the measurements of the parts.

- **UCL** → defines the **highest acceptable height** for the parts  
- **LCL** → defines the **lowest acceptable height** for the parts  

➡️ Ideally, all parts should fall **between these two limits**.

---

## 🧮 The task

Using **SQL window functions** and **nested queries**, we will:

- Analyze **historical manufacturing data**  
- Define the **acceptable range (UCL & LCL)**  
- Identify points in the process that fall **outside the limits**  
- Highlight cases requiring **adjustments**

This ensures a **smooth manufacturing process**, consistently producing **high-quality products**.

---

## 📊 The Data

The dataset is stored in the table **`manufacturing_parts`**, which contains the following fields:

- `item_no` → Item number  
- `length` → Length of the item made  
- `width` → Width of the item made  
- `height` → Height of the item made  
- `operator` → The operating machine  
