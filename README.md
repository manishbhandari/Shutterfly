# Shutterfly
Code Challenge
# Prequsites:

Python 3.0 is required for this code
MySQL is required to save data 

# Assumptions:
Pre built solutions / parser / libraries use wasnt allowed, thus i have tried to re-create a small POC of a text parser. there are many already available.


# Libraries used:
I have used pymysql library in order to connect MYSql database server. 

Liraried which can make it better:
There are many libraries available which can do the task much faster and efficient but i assumed that pre-fabricated solution were not expected.
Therefor i didnt use them. Below mentioned libraries could have worked better in this case
re - for regex
itertools for iterations and work with key value pairs
ast - to convert lists into key value pairs  
pandas - to create data frames and calculate in memory
json - to parse json files.


# SQL:
All sql code resides in *.sql files in 'src' folder. 
There are 1 file for creating objects and another file to populate data.
I am not calling SQL filed from python file because we create DB objects once and there is no point keep checking their existence before every execution


# Test cases which fails:
1) Because of time constraints-  I couldn’t filter fix key value pairs if they occur as column values. For example tags for sitevisit table.
2) I am splitting based on ':' , and improper placement of ':' may end up in bad split of data
3) I couldn’t check for rows already exists in tables before insert and update. I couldn’t finish in time because of work pressure at my current job

# Future challenges
1) data cleansing data needs more work
2) Methodology to parse bad splitters and ignore them is needed.



