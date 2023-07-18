# cs
Cyber Security and Ethical Hacking Internship Program.
CTF CHALLENGE
Introduction:
Capture the Flag (CTF) in cyber security is an exercise in which "flags" are secretly hidden in purposefully vulnerable programs or websites. Security CTFs are usually designed to serve as an educational exercise to give participants experience in securing a machine and conducting and reacting to the sort of attacks found in the real world

- First Scan the ports using nmap tool to find the open port vulnerability
Command: nmap -Sc -Sv 192.168.1.127  
FLAG1: Now as we found the open FTP port, we try to find the flag from there 
Command: ftp anonymous 192.168.1.127
Here we login as anonymous user and check for the flag
Then command: ls 
To check the files and directories in the ftp for there we found the flag1.txt file 
To open that flag, we save that file into the pc using 
Command: get flag1.txt
That fi le saved to the computer and we can see the output below    
 

 







FLAG2: Now we are finding the flag2 to find that flag we uses the dirbuster into the kali box
Command: dirb http://192.168.1.127/
We use dirb to for broute forcing the given ip address  
It shows the hidden directories and the files
From there we found the text file http://192.168.1.127/robots.txt
Open that link into to the web and we found our flag2 as shown below
 


 

















FLAG3: come to flag3 many a time we find the flag from the source code so we try to find the flag from each of the pages to the given site and from there we found the flag from the 3rd page of the site 
http://192.168.1.127/pages/BlogPostComponent.html
from the footer of the html page.

 














FLAG4: flag4 we are using the OWASP Dirbuster tools to find the admin-panel and find in it from admin-panel view response 
 
 
 














FLAG5: flag5 when  we are scanning for the flag4 for the hidden files and directories we found the flag5 its pop up as a warning during the scan 

 















FLAG6: we found the admin-panel login from using dirbuster we open that login page and the using the burpsuite we found the flag6 as show below
http://192.168.1.127/4dm1n/ found this from the dirbuster scan and using that we go to the site and try to log and using burp suite we found the flag6
burpsuite used for performing the web security testin it stop the traffic and request and from that we have to capture our flag 
steps :
step 1: open the  http://192.168.1.127/4dm1n in web
step 2: open the burpsuite and turn on the intercept from proxy 
step 3: the try to end the log in id password 
step 4: then in burpsuite turn off the intercept and then in web press the login
step 5: forward the request in burpsuite the we found our flag6 
 
