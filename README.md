# CODEPATH WEEK 8

BLUE 
Vulnerability 1: SQL INJECTION
	Accomplished by inserting 'OR SLEEP(5)=0--' after id= at the end of a salesperson page URL. Causes the page to do nothing and just load for 5 seconds.

Vulnerability 2: Session Hijacking
	Can be used to log in on two seperate browsers, by logging in on one, copying the session ID and then changing the session id of the unlogged in browser to match the first, causing it to be logged in.

Green
Vulnerability 1: Username Enumeration
	If one attempts to log in with an existing username the failure message displays in bold text. If using a non-existing username it will not be bold.

Vulnerability 2: Cross Site Scripting
	If you insert a script into the contact form. It will be received when logged in as the admin after clicking the feedback button.

RED
Vulnerability 1: Insecure Direct Object Referencing
	At the end of the url for each salesperson there is an id= form. By entering different numbers for the salesperson id (10)you can find a salesperson whose page is not listed for the public. 

Vulnerability 2: CSRF
	On the edit user page, right click and hit inspect. You are able to change the csrf token and still continue on with editing the user, which should not be possible. 
