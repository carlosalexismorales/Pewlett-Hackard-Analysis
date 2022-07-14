# Pewlett_Hackard_Analysis_

Using SQL, PostgreSQL, pgAdmin for a company's database analysis

## Project Overview

The purpose of this analysis is to conduct a Database analysis for Pewlett Hackard. This analysis will achieve two goals:  determiningthe number of future retirees per title and identifying which employees are fit/eligible for the mentorship program. This analysis will also include a report that summarize's the findings to help Pewlett Hackard's upcoming transitional period. 


## Resources

- Data Sources: 
  - departments.csv
 - dept_emp.csv 
 - dept_manager.csv
 - employees.csv 
 - salaries.csv
 - titles.csv

- Resources: 
 - SQL
 - PGAdmin
 - POSTgreSQL 

## Results

- In the image below, a query is written and executed to create a retirement_titles table for employees who are born between January 1, 1952 and December 31, 1955. The number of entries in this table is calculated using SELECT count(emp_no) FROM retirement_titles, which gives a total of 133,776 lines. Because the data comprises more than 130,000 lines, it requires additional filtration before it can be useful to management. Some entries are duplicated since some employees' titles have changed throughout their careers as they moved from one position to another.




- In the image below, another query is written and executed to create a unique_titles tables - this table is modified to be without the duplicates. In this table, we see that there are 90,398 entries. This means that we were able to get closer to the total number of future retirements. This number is still vast, therefore, we need to filter the date even further. 



- In the image below, we create a final table called retiring_titles. As a result, we are able to see the number of retireees in each department. Using this information we can see which departments have the most and least amount of roles to fill. Senior Engineer has the most amount of retirees while Manager has the least amount. This indicates that it is going to be difficult to fulfill those roles since it is a technical and senior position - one that takes a lot of experience and expertise to step into. 



- A final table was created to determine which is there are enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees. 







## Summary

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

There are 90,398 roles that need to be filled. In the image below, we see there are 57,668 are those roles are Senior positions which means that there needs to be internal promotion to fulfill those roles or the company needs to have an extensive hiring process to get people with a high level of expertise and experience on board. 



Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

There are not enough qualified, retirement-ready employees to mentor the next generation. From the unique_titles table, we see that there are not enough. If the company was go ahead with the current number, each employee would have a rather large team to look after and mentor - a feat that can be difficult to accomplish with the proper resources. In the image below, we see a total of 56,859 employees; a number that is below what is needed in order to help mentor and replenish the next generation of employees. 




