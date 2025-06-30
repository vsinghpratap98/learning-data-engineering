### 🧩 What Are Joins in SQL?

**Joins** in SQL are used to **combine rows from two or more tables** based on a **related column** (usually a key). They're essential for working with **normalized databases**, where data is split across multiple related tables.

---

### 🔄 Types of Joins in SQL

Here are the **main types of SQL joins**, with simple explanations and visual mental models:

---

#### 1. **INNER JOIN**

* Returns only the **matching rows** from both tables.
* If there's no match, the row is **excluded**.

**Syntax:**

```sql
SELECT *
FROM Orders o
INNER JOIN Customers c ON o.customer_id = c.customer_id;
```

🧠 *Think: intersection of two circles (common data only).*

---

#### 2. **LEFT JOIN (LEFT OUTER JOIN)**

* Returns **all rows from the left table**, and the **matched rows** from the right table.
* If there's no match in the right table, it returns **NULL** for that side.

**Syntax:**

```sql
SELECT *
FROM Customers c
LEFT JOIN Orders o ON c.customer_id = o.customer_id;
```

🧠 *Think: keep all left side rows, even if there's nothing to match on the right.*

---

#### 3. **RIGHT JOIN (RIGHT OUTER JOIN)**

* Returns **all rows from the right table**, and the **matched rows** from the left.
* If there's no match in the left table, returns **NULL** for that side.

**Syntax:**

```sql
SELECT *
FROM Orders o
RIGHT JOIN Customers c ON o.customer_id = c.customer_id;
```

🧠 *Opposite of LEFT JOIN.*

---

#### 4. **FULL JOIN (FULL OUTER JOIN)**

* Returns **all rows from both tables**.
* Fills in **NULLs** where there's no match on either side.

**Syntax:**

```sql
SELECT *
FROM Customers c
FULL OUTER JOIN Orders o ON c.customer_id = o.customer_id;
```

🧠 *Think: union of all data from both tables.*

---

#### 5. **CROSS JOIN**

* Returns **Cartesian product** of the two tables.
* Every row from table A is combined with **every row** from table B.

**Syntax:**

```sql
SELECT *
FROM Products p
CROSS JOIN Colors c;
```

🧠 *Useful for combinations or permutations.*

---

#### 6. **SELF JOIN**

* A table joins with **itself**.
* You need to use **aliases** to distinguish between the two instances.

**Syntax:**

```sql
SELECT a.employee_id, a.name, b.name AS manager
FROM Employees a
JOIN Employees b ON a.manager_id = b.employee_id;
```

🧠 *Used for hierarchical data like employee-manager or folder-subfolder.*

---

### 🛠️ Practical Use Cases

* `INNER JOIN`: Getting customers who placed orders.
* `LEFT JOIN`: Getting all customers and whether they placed orders.
* `RIGHT JOIN`: Getting all orders, even from non-registered customers.
* `FULL JOIN`: Getting all data, matched or unmatched.
* `CROSS JOIN`: All combinations of sizes and colors.
* `SELF JOIN`: Employee hierarchy or friend-of-a-friend networks.

---

