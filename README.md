# Pewlett-Hackard-Analysis

## Overview of the Analysis

Purpose of the analysis was to submit a report to the company by determining the number of the retiring employees and the employees who will be eligible for the 
mentorship program, in order to inform HR of the job openings to be opened and the preparation to be required to fill these openings in advance. For this report, 
a database composed of 6 csv files was imported, modelled, used to create tables, editted through SQL queries. 

## Results

- In Deliverable 1, the employees who were born between January 1, 1952 and December 31, 1955 were pulled out of the data and ordered by their employee numbers 
to determine the number of employees who would be retired. The table was consisted of employee numbers, first and last names, titles, from date and to date as the 
start and end of employment days. The list of the retiring employees were saved in retirement_titles.csv file.

![ret_tit](https://user-images.githubusercontent.com/104400293/194734102-3ddd29c1-62e9-416b-a129-f08c8ccd5392.PNG)

- Using the retirement titles data, a new query was created by retrieving employee number, first and last names and title columns from retirement titles table. 
As there were duplications in data due to position shifts, the data was needed to be cleared off to get the correct numbers. In this stage, the employees who were 
already retired were also cleared off the list, and eventually with employee numbers, first and last names and duplicate-cleaned titles, a new table was created 
under the file name of unique_titles.csv.

![uniq_tit](https://user-images.githubusercontent.com/104400293/194734104-f1f92519-d58a-4779-99db-fc007ba6bece.PNG)

- In the next step, the number of titles were retrieved from the unique titles table to receive the number of retiring employees from each position. 
A new table named retiring_titles was created with the count of positions with their titles.

![retiring_t](https://user-images.githubusercontent.com/104400293/194734112-c4840b90-d879-4af7-b0a2-f12e01e5b807.PNG)

- In Deliverable 2, a new table was created in order to retrieve the list of the employees who were eligible for the mentorship after retirement. In this step, 
employee number, first and last names, birth dates, start/end employment dates, and title informationn were retrieved from three different tables into 
mentorship_eligibility.csv file. The data was filtered in birth date column into a specific date interval, and table was ordered by the employee number. 

![ment_elig](https://user-images.githubusercontent.com/104400293/194734114-f56b1e1a-2840-4eca-bea0-448146a7e3f0.PNG)

## Summary

According to report, below are the numbers of the positions that will need to be filled after the retirements:

- 57.720 Engineers
- 52.664 Staff
- 50.661 Senior Engineer
- 48.466 Senior Staff
- 8315 Assisstant Engineer
- 4512 Technique Leader
- 14 Manager

The number of the retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees were as follows:
- 501 Engineers
- 156 Staff
- 169 Senior Engineer
- 568 Senior Staff
- 156 Staff
- 77 Tecnique Leader

Report showed that the number of the employees to mentor the next generation of Pewlett Hackard is not enough to cover the requirement in any department.
Additionally, the report showed that, there are no appropriate candidates among the retirement-ready employees to mentor the future managers of the company.
The count of the retirement-ready employees showed that, the positions of Engineers, Senior Engineers, Senior Staff, and Staff are the titles which will be loosing a major number of personnel, which will require attention to be covered 
by new hirings.
