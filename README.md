# JOINS AND AGGREGATE FUNCTIONS
# Introduction:
Joins allow us to combine data from different tables based on a related column between them. This operation is vital for harnessing the full power of a relational database, as it allows us to establish connections between different sets of information. 
There are various types of joins, including INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN, each serving specific purposes in data retrieval.
Aggregate functions, on the other hand, are used to perform calculations on sets of data. 
These functions allow us to derive meaningful insights from our data, such as finding averages, sums, counts, minimum and maximum values, among others. Common aggregate functions include COUNT, SUM, AVG, MIN, and MAX.
By combining joins with aggregate functions, we can unlock the potential for complex data analysis and reporting, enabling us to extract precisely the information we need from our databases.

In this task, I made use of 4 practical business questions to solidify my understanding of SQL joins and aggregate functions.

# Problem Statement:
Come up with 4 business questions and query the tables provided: Ensure to use the following commands;
JOINS
GROUP BY
At least 2 Aggregate Functions
ORDER BY.

# Questions:
1. Calculate the average salary of employees whose yearly increment is 5000. Return average salary.
2. Identify employees whosed yearly increment is greater than 4000; display in desecnding order. Return complete information about the employees
3. Calculate the total sum of the employees yearly increment
4. Identify the employees from the city of Mumbai with their Dept ID, Phone number, Pincode and email.

# Solutions:

![AVERAGE SALARY](https://github.com/alwaysgladys/SQL--TASK-5/assets/144185133/ac7407dc-e19a-4f21-b480-6cbb1d8be477)

This image provided above shows the calculated average salary of the employees whose yearly increment is 5000 and the syntax used is as follows;

SELECT AVG(Salary)  FROM Table_Name WHERE Yearly Increment = 5000 GROUP BY Yearly Increment;



![YEARLY INCREMENT ABOVE 4000](https://github.com/alwaysgladys/SQL--TASK-5/assets/144185133/0c3589e8-3733-40d9-aa17-ee8b2e1c9a99)

This particular image displays the complete information of the employees whose yearlyincrement is greaterthan 4000 in a descending order  The syntax used is as follows;

SELECT * FROM Table_Name WHERE Yearly Increment > 4000 ORDER BY Yearly Incremrnt DESC;


![TOTAL YEARLY INCREMENT](https://github.com/alwaysgladys/SQL--TASK-5/assets/144185133/cb8ed25c-1f58-43b9-b0a8-8108eb5eb228)

The image above displays the total sum of the employees yearly increment and the syntax used is as follows;

SELECT SUM(Increment) as Total Yearly Increment FROM Table_Name;


![EMPLOYEES FROM MUMBAI](https://github.com/alwaysgladys/SQL--TASK-5/assets/144185133/0c81203a-67b1-45ed-8edd-e4987038a351)

This very image displays the names, Dept ID, Phone number, Pincode and email of all the employees from the City of Mumbai and the syntax used is as follows:
SELECT Name, number, pincode, email Dept ID FROM Table_name WHERE City = ""Mumbai" ORDERBY Name;


![joins](https://github.com/alwaysgladys/SQL--TASK-5/assets/144185133/6770eb57-c525-467f-b074-74123adba6d0)

This last image is a pictorial view of how i joined two tables; the employee and salary tables having the EmpID as the unique Number


# Conclusion:
This particular task has highlighted the remarkable potential of SQL in facilitating business queries.

Through a series of business questions and the use of SQL commands like ORDER BY, GROUP BY, and Aggregate functions like COUNT, SUM, AVG, MIN, and MAX, valuable insights were obtained that would help in decision-making within a business context in the near future.
