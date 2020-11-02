# Log_Activity

By: Jay Patel & Dylan Cathcart
This is for our Project 3 developed on Jupyter Notebook written in python3

This is the plan of action for our INST126 Project 3. We will be programming this project in Python. The overall idea of this project is that we will be given a log file which we will have to parse through to find various information.

Suspicious Activities (Function 1)
Within the log file we will need to find the total count of suspicious activities
Data Structure
Dictionary (Dictionary of all users that have been flagged for suspicious activity and the total number of cases per user)
In this function I would need to have something that checks to see how many times a user has logged in more than 5 time on one day or if the user has logged in once between 12 - 5am, if so then those users will have one more case added in the dictionary

Irresponsible Behavior (Function 2)
Track irresponsible behavior of user by checking users log in to log out ratio
Data Structure
Dictionary (Dictionary of all users and how count of irresponsible behaviour per user)
In this function we need to check how many times each user has logged in and out and if the number of log in for a specific user is greater than the number of log outs they will be marked for irresponsible behavior and the number of irresponsible behaviors performed will be added to the dictionary next to the user.

System Glitch (Function 3)
Within the log file, we must find the amount of cases in which a user had more logouts than logins. These instances must be flagged, and listed as a glitch. 
Data Structure
List(A list of all of the instances where a user appears to logout of the system more times than they login.)
For this function, we must write code to determine the amount of glitches that occur in the system. If there is a glitch for a user on a certain day, the count of glitches increases by one. The sum of days in which glitches occurred is the total count for the amount of system glitches. The time, activity, and server information must be listed based on time in which the glitch occurred, in ascending order. 

Domain Count (Function 4)
Within the log file we will need to find all of the unique domains and the number of users registered within each domain, by checking the second part of the users email address. Each domain name should only occur once in the list. 
Data Structure
List (We will be making a list of all of the unique domain names that we find in the log)
For this function, we will need to write code to read the file, and create a list of all of the domains that occur throughout the log. As stated, all of the domains must be unique, so there should be no repeating domain names in the output. 


