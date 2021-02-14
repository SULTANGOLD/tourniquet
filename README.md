## Problem: 
Companies want to incorporate flexible work hours to their workflow. Instead working 8 hours per day, they want to allow their employees to work less/more if the total number of working hours per week is 40. In case an employee works less than 40 hours per week, he needs to compensate those working hours during specified period of time.

## Solution:
The software which tracks and stores an employee work hours.

## Requirements

### Functional requirements:

1. The software should use QR codes for authentication.
2. The server shall generate and keep track of distinct and permanent QR codes for every employee.
3. The software shall have the profiles for each employee.
4. If the total week hours exceed required hours, those hours shall be subtracted from the next week's required work hours.
5. If the total week hours is under required hours, those hours shall be added to the next week's required work hours.
6. Holidays shall be excluded from work hours.
7. Each employee shall be able to manually exclude their hours spent on leisure activities.
8. Each employee shall be able to manually record special reasons for not being at work.
9. The software shall have an admin page for CRUD operations with an access for employers.

### Non-functional requirements:
1. The client application shall be web based.
2. The client application's web pages should be responsive to mobile devices.
3. The client application should load within 10 seconds.
4. The server shall sanitize passed data.
5. The server shall handle 500 employees.

### User requirements:
1. The software shall record employees' work hours (till midnight).
2. The employees shall be able to keep track of their flex status.
3. The software shall account for leisure hours, sick days and holidays.
4. The software shall be accessible for non-IT specialists.

## Implementation
* Programming languages: Python for backend, HTML/CSS/JS for frontend
* Database engine: SQLite

Since our project is just a prototype, we chose SQLite for its simplicity and ease of use. Compared to other database engines such as Oracle, it doesn't require extensive setup and seperate daemon to work but just one file. 
