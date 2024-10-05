# Applying_filters_to_SQL_queries

## Objective

- This project demonstrates how to apply various filters to SQL queries to retrieve specific subsets of data from a database. Filtering data is a fundamental aspect of database management and is crucial for generating meaningful insights from large datasets.
- In this specific project,  It is my job to ensure the system is safe, investigate all potential security issues, and update employee computers as needed. The following steps provide examples of how I used SQL with filters to perform security related tasks.

## Steps

- The following code shown demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.

<div>
    <img src="https://github.com/user-attachments/assets/759d8422-4bb9-40a5-bbe7-c9ab00166a9c" />
</div>

- First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an AND operator to filter my results to output only login attempts that occurred after 18:00 and were unsuccessful. The first condition is login_time > '18:00', which filters for the login attempts that occurred after 18:00. The second condition is success = FALSE, which filters for the failed login attempts.

### Retrieving login attempts on specific dates
- The following code demonstrates how created a SQL query to filter for login attempts that occurred on specific dates.
<div>
    <img src="https://github.com/user-attachments/assets/6b5cc369-d52e-4888-b7dc-a1d05060a1b1" />
</div>

- Started off by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an OR operator to filter my results to output only login attempts that occurred on either 2022-05-09 or 2022-05-08. The first condition is login_date = '2022-05-09', which filters for logins on 2022-05-09. The second condition is login_date = '2022-05-08', which filters for logins on 2022-05-08.

### Retrieve employees in Marketing
- For this project, we need to update the computers for certain employees in the Marketing department. To do the update, I have to get the imformation on which employee computers to update.
- The following code demonstrates how I created a SQL query to filter for employee computers from employees in the Marketing department in the East building.

<div>
    <img src="https://github.com/user-attachments/assets/6033e81a-380e-4157-b754-ad2284db6534" />
</div>

- First, I started by selecting all data from the employees table. Then, I used a WHERE clause with AND to filter for employees who work in the Marketing department and in the East building. I used LIKE with 'East%' as the pattern to match because the data in the office column represents the East building with the specific office number. The first condition is the department = 'Marketing' portion, which filters for employees in the Marketing department. The second condition is the office LIKE 'East%' portion, which filters for employees in the East building.

## Summary
- I applied filters to SQL queries to get specific information on login attempts and employee computers. I used two different tables, log_in_attempts and employees. I used the AND, OR, and NOT operators to filter for the specific information needed for each task. I also used LIKE and the percentage sign (%) wildcard to filter for patterns.

## Skills Learned
- Through this project, I gained valuable skills in SQL query optimization and data manipulation. I learned how to apply various filters to extract specific data subsets, enhancing my ability to handle complex queries using WHERE, AND, OR, and NOT operators.
