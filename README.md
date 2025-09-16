# Database Design and Normalization

*  **Understand the principles of good database design** and **normalization**.
  
### Query 1 Achieving 1NF 
- given the following table **ProductDetail**:

| OrderID | CustomerName  | Products                        |
|---------|---------------|---------------------------------|
| 101     | John Doe      | Laptop, Mouse                   |
| 102     | Jane Smith    | Tablet, Keyboard, Mouse         |
| 103     | Emily Clark   | Phone                           |


- **An SQL query** to transform this table into **1NF**, ensuring that each row represents a single product for an order

--- 

### Query 2 Achieving 2NF 

- given the following table **OrderDetails**, which is already in **1NF** but still contains partial dependencies:

| OrderID | CustomerName  | Product      | Quantity |
|---------|---------------|--------------|----------|
| 101     | John Doe      | Laptop       | 2        |
| 101     | John Doe      | Mouse        | 1        |
| 102     | Jane Smith    | Tablet       | 3        |
| 102     | Jane Smith    | Keyboard     | 1        |
| 102     | Jane Smith    | Mouse        | 2        |
| 103     | Emily Clark   | Phone        | 1        |


- **An SQL query** to transform this table into **2NF** by removing partial dependencies. Ensure that each non-key column fully depends on the entire primary key.
