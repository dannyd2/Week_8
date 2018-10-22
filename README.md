# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration 
* Insecure Direct Object Reference (IDOR) 
* SQL Injection (SQLi) 
* Cross-Site Scripting (XSS) 
* Cross-Site Request Forgery (CSRF) 
* Session Hijacking/Fixation 

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection --> The blue site has an SQL vulnerability by displaying the message "database query failed". This was proven by a sleep command in the url. 
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_1_BLUE.gif" width="800">

Vulnerability #2: Session Hijacking/Fixation --> By using the session ID tool that is provided by codepath, as well as Burpsuite, we can change the session ID to the one we got from the victims. The attacker then appears to be the victim and is able to log in.
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_2_BLUE.gif" width="800">

## Green

Vulnerability #1: XSS --> One can perform an XSS attack on the 'Contact' page of the website. Once an Admin checks their feedback page, the script executes. 
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_2_GREEN.gif" width="800">


Vulnerability #2: User Enumeration --> When a known username is enetered (any password may be entered) the message "Log in was unsuccessful." appears in BOLD. However, when a non existing username is entered, "Log in was unsuccessful." is not in bold. 
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_1_GREEN.gif" width="800">

## Red

Vulnerability #1: CSRF --> Salesperson info without correct CSRF value can be updated on the red site, however the other sites do not allow the salesperson info to be updated without the correct CSRF value.
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_1_RED.gif" width="800">

 
Vulnerability #2: IDOR --> While on the 'Find a salesperson' tab, you can edit the 'id' field in the URL tp expose a salesperson whose not supposed to be exposed. 
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_2_RED.gif" width="800">


## Notes

Describe any challenges encountered while doing the work

