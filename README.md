# Pewlett-Hackard-Analysis
## Overview
In order to prepare for a "silver tsunami", a manager at a large company known as Pewlett-Hackard requires an employee database to be constructed from various existing csv files in order to determine how many employees, by position, will be retiring in the near future as well as how many of those employees are eligible for a mentorship program to help train oncoming employees.

## Results
- There are 72458 employees who are currently at the company will be retiring.

- The number of employees retiring by title are as follows:

![image](https://user-images.githubusercontent.com/112590378/195482859-429d8c78-b562-408e-9444-e8f147f8a87c.jpeg)

- 1549 employees are eligible for the mentorship program.

## Summary
According to the table, most of the retiring personel are part of the Senior Engineers or other Senior Staff.  The company should put the most effort into training or seeking employees for these roles.

Another query and corresponding table that would give them more insight on how to proceed is the following: 

```SELECT count(title) "count", title
INTO mentorship_titles
FROM mentorship_eligibility
GROUP BY title
ORDER BY count DESC
```


![image](https://user-images.githubusercontent.com/112590378/195486287-34855db5-372f-475b-9880-5271db2176f7.jpeg)
