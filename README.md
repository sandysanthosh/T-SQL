Transact-SQL (T-SQL) is a Microsoft SQL Server's proprietary extension to the SQL (Structured Query Language). It encompasses SQL's data manipulation and data definition language with additional programming constructs to enhance its functionality. T-SQL is used for querying, modifying, and managing data in SQL Server databases.

### Features of Transact-SQL:

1. **Data Manipulation Language (DML)**:
   - T-SQL includes standard SQL commands for retrieving, inserting, updating, and deleting data from tables using commands like `SELECT`, `INSERT`, `UPDATE`, `DELETE`.

2. **Data Definition Language (DDL)**:
   - T-SQL provides DDL statements for defining and managing database objects such as tables, indexes, views, stored procedures, and triggers. Commands like `CREATE`, `ALTER`, `DROP` are used for these purposes.

3. **Procedural Programming Constructs**:
   - T-SQL offers procedural programming capabilities with constructs like variables, control-of-flow statements (IF-ELSE, WHILE loops), and error handling (TRY-CATCH blocks), making it more than just a query language.

4. **Stored Procedures, Functions, and Triggers**:
   - It supports the creation of stored procedures (T-SQL scripts saved on the server), functions (scalar and table-valued), and triggers (actions executed in response to specific events).

5. **Transactions**:
   - T-SQL allows managing transactions using `BEGIN TRANSACTION`, `COMMIT TRANSACTION`, `ROLLBACK TRANSACTION` statements to ensure data integrity and consistency.

6. **Error Handling**:
   - Error handling is facilitated through constructs like `TRY-CATCH` blocks to handle exceptions and errors within the scripts.

7. **Views**:
   - Views can be created using T-SQL to represent a subset of data or a logical table based on a query.

8. **Dynamic SQL**:
   - It allows constructing SQL statements dynamically and executing them at runtime using strings concatenated together.

9. **Common Table Expressions (CTE)**:
   - T-SQL supports CTEs, enabling temporary result sets within a query to simplify complex queries.

10. **Window Functions**:
    - Window functions provide capabilities to perform calculations across a set of rows related to the current row.

11. **Full-text Search**:
    - T-SQL provides full-text search capabilities for querying large amounts of textual data efficiently.

### Example of T-SQL:

```sql
-- Creating a sample table
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    FirstName NVARCHAR(50),
    LastName NVARCHAR(50),
    Salary DECIMAL(10, 2)
);

-- Inserting data into the table
INSERT INTO Employees (EmployeeID, FirstName, LastName, Salary)
VALUES (1, 'John', 'Doe', 50000),
       (2, 'Jane', 'Smith', 60000);

-- Retrieving data using SELECT statement
SELECT * FROM Employees;

-- Example of a stored procedure
CREATE PROCEDURE GetEmployeeByID
    @EmpID INT
AS
BEGIN
    SELECT * FROM Employees WHERE EmployeeID = @EmpID;
END;
```

T-SQL plays a significant role in managing and manipulating data within Microsoft SQL Server, providing not only SQL functionalities but also programming capabilities to create robust database solutions. Understanding T-SQL is crucial for working effectively with SQL Server databases.
