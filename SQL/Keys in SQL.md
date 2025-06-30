In SQL (Structured Query Language), **keys** are special fields (columns) in a table that help uniquely identify rows and establish relationships between tables. They're called **"keys"** because they act like a *key to unlock* access to data—just like a key opens a specific door, a key in SQL identifies a specific row or connects related rows across tables.

---

### 🔑 **Types of Keys in SQL**

Here are the most commonly used types of keys:

1. **Primary Key**

   * Uniquely identifies each row in a table.
   * **Must be unique and NOT NULL**.
   * Each table can have **only one** primary key.
   * Example:

     ```sql
     CREATE TABLE Students (
       student_id INT PRIMARY KEY,
       name VARCHAR(100)
     );
     ```

2. **Foreign Key**

   * A column that creates a link between two tables.
   * It refers to the **primary key in another table**.
   * Ensures **referential integrity**.
   * Example:

     ```sql
     CREATE TABLE Enrollments (
       student_id INT,
       FOREIGN KEY (student_id) REFERENCES Students(student_id)
     );
     ```

3. **Candidate Key**

   * A column or group of columns that can qualify as a unique key.
   * A table can have multiple candidate keys, but only one is chosen as the **primary key**.

4. **Composite Key**

   * A **primary key made up of more than one column**.
   * Used when a single column cannot uniquely identify a row.
   * Example:

     ```sql
     CREATE TABLE Orders (
       order_id INT,
       product_id INT,
       PRIMARY KEY (order_id, product_id)
     );
     ```

5. **Alternate Key**

   * Candidate keys that were **not chosen** as the primary key.
   * They're still capable of uniquely identifying rows.

6. **Unique Key**

   * Ensures all values in a column are unique (like primary key) but **can contain NULL values**.
   * Example:

     ```sql
     CREATE TABLE Users (
       email VARCHAR(100) UNIQUE
     );
     ```

---

### 🔍 Why the Term “Key”?

* Think of **"key" as an identifier or access tool**.
* It originates from database theory, where a key is the minimal set of attributes required to **uniquely identify a tuple (row)**.
* In relationships (like foreign keys), the key **connects** two tables like a lock-and-key system.

---

