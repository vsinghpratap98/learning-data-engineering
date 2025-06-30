```markdown
# Database Fundamentals

---

## 📘 What is a Schema?

A **schema** is the **structure or blueprint** of a database. It defines how data is organized and how the relationships between data are managed.

- Contains definitions of tables, columns, data types, indexes, views, procedures, and more.
- Helps maintain **data integrity** and **organization**.
- Example: In an e-commerce database, the schema might include `Users`, `Orders`, `Products`, and their relationships.

---

## 🗄️ What is a Database?

A **database** is a **collection of organized data** that can be easily accessed, managed, and updated. It is typically controlled by a **Database Management System (DBMS)**.

- Stores data in structured formats (tables, documents, key-value pairs, etc.).
- Allows CRUD operations: **Create, Read, Update, Delete**.
- Can be relational (SQL) or non-relational (NoSQL).

---

## 🏛️ Differences Between Legacy and Modern Databases

| Feature | Legacy Databases | Modern Databases |
|--------|------------------|------------------|
| **Architecture** | Monolithic | Cloud-native / Microservices |
| **Scalability** | Vertical only (scale-up) | Horizontal (scale-out) |
| **Interface** | CLI or older GUIs | Web UI, APIs |
| **Storage** | On-premises | Cloud-first (AWS, GCP, Azure) |
| **Data Models** | Mostly relational | Supports relational + non-relational |
| **Examples** | IBM DB2, Oracle 9i | PostgreSQL, MongoDB, Snowflake |

---

## 🔁 Differences Between Relational and Non-Relational Databases

| Feature | Relational Databases (RDBMS) | Non-Relational Databases (NoSQL) |
|--------|-------------------------------|----------------------------------|
| **Data Structure** | Tables with rows and columns | Documents, key-value, wide-column, or graph |
| **Schema** | Fixed, predefined | Flexible, schema-less |
| **Scalability** | Vertical | Horizontal |
| **Query Language** | SQL | Varies (MongoDB uses JSON-like queries, etc.) |
| **Transactions** | Strong ACID compliance | BASE (eventual consistency) |
| **Use Cases** | Banking, ERP, CRM | Big Data, IoT, real-time apps |
| **Examples** | MySQL, PostgreSQL, Oracle | MongoDB, Cassandra, Redis, DynamoDB |

---

## 📚 Summary

- A **schema** defines the structure of a database.
- A **database** is where structured or unstructured data is stored and managed.
- **Legacy databases** are traditional, often slower to scale and modernize.
- **Modern databases** support distributed systems, are cloud-friendly, and fit dynamic needs.
- **Relational databases** are structured and reliable, while **non-relational databases** offer flexibility and performance for unstructured or semi-structured data.

---
```

