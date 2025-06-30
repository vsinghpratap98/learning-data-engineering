### 🔤 What is `ENUM` in SQL?

In SQL, an **`ENUM`** (short for **enumeration**) is a **data type** that allows a column to have one value from a **predefined set of values**.

---

### 🧠 Think of `ENUM` as:

> A column that can only accept values from a fixed list, like a dropdown menu in a form.

---

### ✅ Example:

```sql
CREATE TABLE Products (
  product_id INT PRIMARY KEY,
  low_fats ENUM('Y', 'N'),
  recyclable ENUM('Y', 'N')
);
```

Here:

* `low_fats` can only be `'Y'` or `'N'`
* `recyclable` can only be `'Y'` or `'N'`

---

### 📌 Why Use `ENUM`?

* Ensures **data consistency** (only allowed values are entered).
* **Saves storage** space in some databases (like MySQL).
* Makes data more **readable** and **meaningful**.

---

### ❗ Caveats:

* Not supported in all databases (e.g., **PostgreSQL uses `CHECK` constraints or `ENUM` types defined separately**).
* Hard to extend (changing the list of allowed values often requires altering the table).
* Can be less portable across different database systems.

---

### 🆚 ENUM vs CHECK Constraint

| Feature                  | ENUM           | CHECK Constraint               |
| ------------------------ | -------------- | ------------------------------ |
| Type safety              | Yes            | Yes                            |
| Flexibility              | Low            | High                           |
| Supported in             | MySQL, MariaDB | PostgreSQL, SQL Server, Oracle |
| Add/remove values easily | No             | Yes (via altering the check)   |

---
