# passwordchecker
This script uses haveibeenpwned api to see if any of the given passwords
are contained in a data breach. Simply put, it will check 
if your passwords have ever been hacked. 

You will need python3 and requests module installed.

The way this works: It will first hash the password with SHA-1 algorithim and for security, 
only provide the api with first 5 letters of the hashed password(k anonymity). Then the api will 
give all the hashed passwords that match the first 5 letters. Finally, it will compare it with the rest of the hashed password.

How to use it: From the command line/terminal, enter as many passwords as you want as arguments. 

ex) python3 checkmypass.py password123 testpassword1 passwordtest123 