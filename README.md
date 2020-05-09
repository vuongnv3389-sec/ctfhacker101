# ctfhacker101
Note: The number of each flag is the order in which i found it
## Micro-CMS v1
# Micro-CMS v1-flag0
edit the Title of a page and inject a html element, and then the respone shown in below 
![Micro-CMSv1-flag1](https://github.com/vuongnv96/ctfhacker101/blob/master/Micro-CMS%20v1-flag0.png)
# Micro-CMS v1-flag1
Edit the body of a page and inject a html element, and then the response shown in below 
![Micro-CMSv1-flag1](https://github.com/vuongnv96/ctfhacker101/blob/master/Micro-CMS%20v1-flag1.png)
# Micro-CMS v1-flag2
be sure you have check all parameter in edit request
![Micro-CMSv1-flag1](https://github.com/vuongnv96/ctfhacker101/blob/master/Micro-CMS%20v1-flag2.png)
# Micro-CMS v1-flag3
find forbidden page
![Micro-CMSv1-flag1](https://github.com/vuongnv96/ctfhacker101/blob/master/Micro-CMS%20v1-flag3-0.png)
and find a way to access forbidden page
![Micro-CMSv1-flag1](https://github.com/vuongnv96/ctfhacker101/blob/master/Micro-CMS%20v1-flag3-1.png)

## Micro-CMS v2
# Micro-CMS v2-flag0
This version have a login page, when i access a edit page, the server will redirect to login page. How to bypass the authen function. i try some SQLi injection payload, so Bingo.
If wrong username/passwpord, the reponse is 'Unknown user' message. Howerver, when i typed  admin' or '1'='1 into username input, i got 'Invalid password' but password field is not seem to be vulnerable.
Basically, i got an account of admin group by SQLmap tool. Login by this accouct i got first flag of this challenge
# Micro-CMS v2-flag1
And i kept dumping db, i found an second flag in page id 3. normally, i don't have the permission to access this page 
# Micro-CMS v2-flag2
Althought,  i had a admin account but i stilled can't not access the edit page by the GET method. So i tried the POST method and the third flag appeared, OH! That was easier than i thought
