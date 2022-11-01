# Pewlett_Hackard_Analysis_

Using SQL, PostgreSQL, pgAdmin for a company's database analysis

## Project Overview

The purpose of this analysis is to conduct a Database analysis for Pewlett Hackard. This analysis will achieve two goals:  determining the number of future retirees per title and identifying which employees are fit/eligible for the mentorship program. This analysis will also include a report that summarize's the findings to help Pewlett Hackard's upcoming transitional period. 


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


<img width="915" alt="Screen Shot 2022-07-13 at 8 45 21 PM" src="https://user-images.githubusercontent.com/102444078/178893671-08ed1dbb-0ecd-4b7b-9a7b-be964cc54e39.png">



- In the image below, another query is written and executed to create a unique_titles tables - this table is modified to be without the duplicates. In this table, we see that there are 90,398 entries. This means that we were able to get closer to the total number of future retirements. This number is still vast, therefore, we need to filter the date even further. 



<img width="758" alt="Screen Shot 2022-07-13 at 8 46 15 PM" src="https://user-images.githubusercontent.com/102444078/178893774-7ef9e7da-10cf-4720-9149-feb46635430a.png">



- In the image below, we create another table called retiring_titles. As a result, we are able to see the number of retireees in each department. Using this information we can see which departments have the most and least amount of roles to fill. Senior Engineer has the most amount of retirees while Manager has the least amount. This indicates that it is going to be difficult to fulfill those roles since it is a technical and senior position - one that takes a lot of experience and expertise to step into. 



<img width="736" alt="Screen Shot 2022-07-13 at 8 47 04 PM" src="https://user-images.githubusercontent.com/102444078/178893863-32475d42-20b8-4b83-8e30-a7e859838290.png">



- A final table was created to determine which is there are enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees. 



<img width="751" alt="Screen Shot 2022-07-13 at 8 47 36 PM" src="https://user-images.githubusercontent.com/102444078/178893925-bfbc675f-d19f-4721-b8d9-b2e9ebca861b.png">




## Summary

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

There are 90,398 roles that need to be filled. In the image below, we see there are 57,668 are those roles are Senior positions which means that there needs to be internal promotion to fulfill those roles or the company needs to have an extensive hiring process to get people with a high level of expertise and experience on board. 


<img width="199" alt="Screen Shot 2022-07-13 at 8 48 59 PM" src="https://user-images.githubusercontent.com/102444078/178894110-ed249639-559e-43be-af6f-7b568b3995d5.png">



Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

There are not enough qualified, retirement-ready employees to mentor the next generation. From the unique_titles table, we see that there are not enough. If the company was go ahead with the current number, each employee would have a rather large team to look after and mentor - a feat that can be difficult to accomplish with the proper resources. In the image below, we see a total of 56,859 employees; a number that is below what is needed in order to help mentor and replenish the next generation of employees. 


<img width="762" alt="Screen Shot 2022-07-13 at 8 48 07 PM" src="https://user-images.githubusercontent.com/102444078/178894011-e6d111b8-4096-45cb-9241-2ac75d8708d4.png">


