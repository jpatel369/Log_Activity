# Log_Activity

By: Jay Patel & Dylan Cathcart
This is for our Project 3 developed on Jupyter Notebook written in python3

This is the plan of action for our INST126 Project 3. We will be programming this project in Python. The overall idea of this project is that we will be given a log file which we will have to parse through to find various information.

Suspicious Activities (Function 1)
Within the log file we will need to find the total count of suspicious activities Data Structure Dictionary (Dictionary of all users that have been flagged for suspicious activity and the total number of cases per user).  In this function I would need to have something that checks to see how many times a user has logged in more than 5 times in one day or if the user has logged in once between 12 - 5am, if so then those users will have one more case added in the dictionary. First, I created the opening of a new file which all of the data I collected could be added to, and saved to at the end. I then arranged the log so that I could break it down to search for names, activity, e-mail address, and so on. From there, I was able to track the amount of times a user had logged in at a suspicious time, as well as if they have logged in more than 5 times in a day. Whenever either of these activities occurred, they were added to the list, and the file was eventually closed once every user login was checked. 

Irresponsible Behavior (Function 2)
Track irresponsible behavior of user by checking users log in to log out ratio Data Structure Dictionary (Dictionary of all users and how count of irresponsible behaviour per user) In this function we need to check how many times each user has logged in and out and if the number of log in for a specific user is greater than the number of log outs they will be marked for irresponsible behavior and the number of irresponsible behaviors performed will be added to the dictionary next to the user. By using the same method I used in the first question to rearrange, and read the user.log, I just had to change the variables in which we were looking in for abnormalities. Any time a user had more logins than log-outs, it was added to the file of users that exhibited irresponsible behavior. 

System Glitch (Function 3)
For this function, we must write code to determine the amount of glitches that occur in the system. If there is a glitch for a user on a certain day, the count of glitches increases by one. The sum of days in which glitches occurred is the total count for the amount of system glitches. The time, activity, and server information must be listed based on time in which the glitch occurred, in ascending order. So for this I went in and got the necessary information from the log file such as the user email, whether it was a login or logout attempt, etc. Once I had this information I compared the logouts to the logins of each user and for any user that had more logouts and login was added to my system_glitch.txt

Domain Count (Function 4)
For this function, we will need to write code to read the file, and create a list of all of the domains that occur throughout the log. As stated, all of the domains must be unique, so there should be no repeating domain names in the output. What I did for this once I got all the information from the .log file, and separated it by the user's email, time, login or logout, etc. I then pulled only the domains from the users emails. Once I had the domains I compared the number of times each domain was used in the users emails and every time it was seen in an email 1 was added to the counter. Once each domain had been counted I went in and added this information to my new domain_count.txt file.

ERRORS: 
1. When we began working on suspicious activities, the most challenging part was figuring out how to manipulate the user.log in order to sort through it, and arrange it to give us our desired output. I was very lost, and even resorted to counting individual characters to see where certain variables in the user.log started and finished. We were able to overcome this by using strip() to remove unwanted characters or spaces, and separating only the variables we needed from the log. 

2. One error/problem I ran into while working on this project during the system glitch portion was towards the end of my code when I wanted to write all the new information into the system_glitch.txt file, however since my log information was split up into multiple values I didn’t know how to organize this information and write it into the file properly. How I went about solving the problem is by speaking with my partner who had done something similar for the irresponsible behavior function.

3. Throughout the entirety of the project, as two people who are somewhat new to coding, we both ran into a variety of small errors time and time again. Whether the error had to do with indentation, spacing, making sure we had colons after our for loops, or trying to remember which specific function to use, we both had instances where we did not know how to move past a small error for short or long periods of time. We often overcame these issues by working together and going through the whole debugging process by running the code, and trying different ideas to fix our issues. 


