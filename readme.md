# **Skarlet**
### *The Definitive Edition of Kasper DB*

---

## **What is Skarlet?**

Skarlet is a **reference-friendly object store**, designed for developers who need speed, simplicity, and intuitive handling of complex data structures. Think of it as a **friendlier version of Redis**—one that simplifies storing and managing references while retaining **blazing-fast performance**.

With built-in support for object references and its own form of **data normalization**, Skarlet makes reference-friendly querying a breeze. Its learning curve is minimal, so you can hit the ground running.

---

## **Core Features**

### **Complex Data Structures**
- Skarlet supports various complex data structures, including **sets**, **lists**, and **dictionaries**.
- These structures make it easy to model complex relationships and nested data scenarios without losing simplicity or performance.

### **Reference Support**
- Skarlet allows you to maintain **references** to other data structures, enabling you to create sophisticated, interconnected data models.
- References facilitate a normalization approach that avoids deeply nested, hard-to-manage structures.

---

## **Skarlet Normalization Levels**

Skarlet employs a series of normalization "levels" that help maintain a clean, logical data model. These are inspired by normal forms in relational databases but adapted to the key-value and reference-based nature of Skarlet.

**Level 1: Baseline Key-Value Structure**
- **Key-Value Model**: Skarlet stores data as keys and values within a top-level container called a **node**.
- **Nodes as Collections**: Each node resides in the global space and can be treated like a "table" or "collection."
- **Keys**: All keys must be **strings**—no exceptions. Keys cannot be complex or primitive other than strings.
- **Values**: Values can be either **primitive** or **complex**. Primitive types (integers, reals/floats, strings, and references) form the baseline data representation.

**Level 2: Structuring Complex Data**
- **Complex Data Types**: Values can include complex data structures like sets, lists, and dictionaries.
- **Primitive Containment**: Complex data types can hold any primitive data type (integers, reals, strings, references) within them.
- **No Complex Nesting**: A complex data type cannot directly hold another complex data type. This restriction encourages clearer data modeling, preventing excessive nesting.

**Level 3: Reference-Based Normalization**
- **References as Primitives**: References are considered a special kind of primitive data type. They can point to other complex data structures or primitive values, acting as links rather than containers.
- **Avoiding Deep Nesting**: By using references, you maintain a normalized structure. Instead of embedding one complex object inside another, you reference it, resulting in a cleaner, more maintainable model.
- **Flexible Linking**: References enable relational-like linkage without forcing rigid schema constraints, combining the flexibility of key-value stores with the organizational benefits of normalized data models.

---

By following these normalization levels, you can leverage Skarlet’s powerful features—complex data structures, references, and key-value simplicity—while maintaining a clear, logical, and high-performance data design.

## **Other Features Skarlet Promises**:
- **Better documentation**: Comprehensive and clear, to get you started faster.
- **Better drivers**: Reliable, performant, and developer-friendly.
- **Better reference support**: Seamlessly manage object relationships and queries.
- **Faster than Kasper**: Optimized to perform at lightning speed.
- **More lightweight than Kasper**: Efficient and easy to deploy.

---

## **What Happened to Kasper?**

Kasper was my first attempt at creating a database during my sophomore year of college. While it was ambitious and innovative at the time, it tried to do too much—following the footsteps of Redis, SQL, and Neo4j. This led to a **bloated and hard-to-use system**.

Recognizing its shortcomings, I decided to start from scratch. Skarlet is the result: a focused, refined, and vastly improved version of Kasper. It keeps the essence of what made Kasper unique while delivering on the promise of **speed**, **simplicity**, and **practicality**.

---

## **Why Choose Skarlet?**

Skarlet isn’t just another object store—it’s a tool designed to help developers work smarter, not harder. Whether you're building a blazing-fast web app, a data-intensive API, or anything in between, Skarlet’s focus on **speed** and **reference management** makes it the perfect choice.

---

Get started with Skarlet today and experience the **definitive edition** of Kasper DB! 🚀

--- 
