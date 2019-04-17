Week 9 Project: Pentesting Live Targets     
Time spent: 8 hours spent in total   

The six possible exploits are:  
  
Username Enumeration  
Insecure Direct Object Reference (IDOR)  
SQL Injection (SQLi)  
Cross-Site Scripting (XSS)  
Cross-Site Request Forgery (CSRF)  
Session Hijacking/Fixation   

BLUE   
Vulnerability #1: SQL Injection   
gif: blue1   
In the GIF, we can enter an AND clause and if we set it to a false boolean value, then we will be redirected to the directory as Blue makes sure to redirect for ids that are not found.    
Vulnerability #2: Session Hijacking/Fixation     
gif: blue2    
Using two different browsers, one acting as a normal user and one as a staff user, changing the session id on the normal user's browser to the staff user's session will give access to the staff menu.     

RED  
Vulnerability #1: Insecure Direct Object Reference    
gif: red1    
GIF show an attacker getting access to the hidden user's accounts that the attacker is not permitted to view.    
This is done through modifying the "id" parameter in the URL's to change the GET request.    
Vulnerability #2: Cross-Site Request Forgery (CSRF)     
gif:red2    
The site accepts a post request from a different source that has a hidden form in it, and makes alterations to the user database.      

GREEN   
Vulnerability #1: Username Enumeration    
gif：green1     
When using a nonexistent username and a random password, the site's error message states "Log in was unsuccessful.". However, when using an existing/valid username and a random password, it shows the error message, but in bold "Log in was unsuccessful.".    
Vulnerability #2: Cross-Site Scripting (XSS)     
gif:green2    
This site's feedback form has a stored xss alert vulnerability.     
