Here's a comprehensive list of **interview questions related to SQL keys** commonly asked in **data engineering** roles at tech companies. These range from basic to advanced, including real-world use cases.

---

## ✅ **Basic-Level Questions**

These check your understanding of key concepts and definitions.

1. **What is a key in SQL?**
2. **What is the difference between a primary key and a unique key?**
3. **Can a table have more than one primary key?**
4. **What is a foreign key, and why is it important?**
5. **Can a foreign key be null or duplicate?**
6. **What happens if you try to insert a foreign key value that doesn’t exist in the parent table?**
7. **What is the difference between a primary key and a foreign key?**
8. **Can a primary key be NULL? Why or why not?**
9. **What is a composite key? Give an example.**
10. **What is a candidate key? How is it different from a primary key?**
11. **What is an alternate key?**
12. **What is a surrogate key and how is it different from a natural key?**
13. **What is a unique constraint? How is it different from a unique key?**
14. **What is the purpose of a key constraint in relational databases?**

---

## 🔄 **Intermediate / Scenario-Based Questions**

These test practical applications and your understanding of key constraints in real-world database design.

15. **Suppose you have a table with no primary key. What problems could arise?**
16. **How would you enforce data integrity between two tables?**
17. **What is the best approach to model many-to-many relationships using foreign keys?**
18. **Can two tables have the same primary key value? Explain with context.**
19. **How would you design a schema for customer orders and products using appropriate keys?**
20. **What happens if a foreign key reference is deleted in the parent table?**
21. **What are ON DELETE CASCADE and ON UPDATE CASCADE? Explain with an example.**
22. **Why are foreign keys sometimes avoided in big data pipelines or denormalized tables?**
23. **How do you implement relationships in a star schema without traditional foreign keys?**

---

## 🚀 **Advanced / System Design-Oriented Questions**

These test your knowledge of key design in large-scale systems, data modeling, and performance.

24. **In a data lake or distributed environment, how would you ensure referential integrity without foreign key constraints?**
25. **What are the trade-offs of using natural keys vs surrogate keys in dimension tables?**
26. **How do primary and foreign keys impact database indexing and query performance?**
27. **What happens to indexes when a primary key is dropped or modified?**
28. **How would you generate surrogate keys in a distributed system (e.g., Spark + Hive)?**
29. **How do you maintain uniqueness in distributed databases where primary keys are not enforced?**
30. **What are hash-based keys and when would you use them over surrogate or natural keys?**
31. **How would you handle key collisions in a large-scale ETL pipeline?**

---

## 📊 **Bonus: SQL Coding-Based Key Questions**

32. Write SQL to create a table with a composite primary key.
33. Write SQL to add a foreign key constraint after a table has been created.
34. How do you drop a foreign key constraint?
35. How would you write a query to find orphan records (child rows with no matching parent)?
36. Show an example of a self-referencing foreign key.
37. Given a table schema, identify the best candidate key(s).

---

