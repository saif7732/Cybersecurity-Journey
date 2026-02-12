#Room: Linux Fundamentals part 3 / Task-4

##Objective: connecting to a pc remotely and flag capturing

Command used: ssh, cd, ls, scp, wget

Steps

Firstly we have to connect to the machine we are attacking using the “ssh user@userIP” command and then enter the password of the user.
<img width="784" height="391" alt="Screenshot 2026-02-11 161041" src="https://github.com/user-attachments/assets/3217d9e6-332a-467d-b7cd-412652e4b4ee" />


After enter the password (given in the task which is “tryhackme”) we will see something like this:
---
---
---
---
---
---
---
---
---
---
---
---
---
---
---
Now our goal is to download the flag.txt from the remote pc (tryhackme) by running the server.
---
---
Then we just have to download the file using the “wget sourceaddress” command.
---
---
Now that we have the file in our pc, we can easily check the content of the file. Since it is a .txt file we can print all data from it using the “cat filename” command.
---
