# Pewlett-Hackard-Analysis
Analyzing retirement data of fictional "Pewlett-Hackard" firm using Postgres SQL.

## Analysis Overview
The purpose of this analysis is to create two tables: one to determine the number of retiring employees and their position titles, and the other to identify employees who are eligible to participate in a mentorship program. Within the first table, we included information such as employee number, first and last name, position title, and start and end date. In the second, we added employee number, first and last name, birth date, start and end date, and position title. 

## Results
* The first table that determines the number of retiring employees and their position titles can be viewed here: [retiring_titles.csv]()

* The second table that identifies employee who are eligible for the mentorship program can be viewed here: [mentorship_eligibility.csv]()

After analyzing the tables of retiring employees and those eligible for mentorships, we can see four key import insights about Pewlett-Hackard:

1) Among retirees, one-third are listed as Senior Engineers, while another third are part of the Senior Staff. This large 'brain drain' of talent at the top of the firm can be important for those looking for promotions, and for potentially bringing in outside talent to temporarily fill the holes of those retiring.
2.) As a result, Senior Engineer and Senior Staff positions have the greatest priority when it comes to deciding which roles the company would like to fill.
3.) Among those that are retiring, there are 1,549 employees that qualify for the mentorship program.
4.) There are more people retiring than there are potential mentors, which means that the company would have to create an efficient program that can cover the disparity between the number of people retiring and the number of people who can be trained to fill these positions. Pewlett-Hackard may want to consider hiring outside talent for senior positions if this disparity of personell leaving, and those needing mentorship is too great.

## Summary
To determine how many roles will need to be filled as the "silver tsunami" of retirees begins to impact Pewlett-Hackard, we can create a graph to categorize the retirees into age groups. For each year, the company can hire (internally or externally) the amount of people that would be retiring, assuming that the retirement age is 65. Currently, we have a list of people who were born between 1952 and 1955. Therefore, we would have a different hiring quota for each of the following four years.

Looking at the current projection of potential mentors and the amount of people retiring, we do not have enough retirees to mentor the next generation of employees. Moving forward, we can create a query that gives us a list of people who are retiring at the end of the current year (and for each following year). From there, the company can prioritize how many younger employees need to be trained to fill up the retired positions. It would also be beneficial if we created a query that grouped mentor-eligible employees into position titles. With this table, the company can plan the mentorship program, specifically, how many mentees a mentor can take on to fulfill the retired roles. 

These insights and recommendations are based off of Pewlett-Hackard wanting to maintain a similar level of personell as they are currently utilizing. If Pewlett-Hackard projects needs for growth, then the mentorship program by iteself will not be enough, and the idea of hiring outside personell to fill those inevitable gaps will be needed.
