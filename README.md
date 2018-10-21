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

Vulnerability #1: SQL Injection
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_1_BLUE.gif" width="800">
--> The blue site has an SQL vulnerability by displaying the message "database query failed". This was proven by a sleep command in the url. 

Vulnerability #2: Session Hijacking/Fixation
<img src="https://github.com/dannyd2/Week_8/blob/master/Exploit_2_BLUE.gif" width="800">
--> By using the session ID tool that is provided by codepath, as well as Burpsuite, we can change the session ID to the one we got from the victims. The attacker then appears to be the victim and is able to log in.

## Green

Vulnerability #1: __________________

Vulnerability #2: __________________


## Red

Vulnerability #1: __________________

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work

