# <p align="center"> Room: Linux Fundamentals part 3 / Task-4 </p>
---

## Objective: connecting to a pc remotely and flag capturing

## Command used: `ssh`, `cd`, `ls`, `scp`, `wget`

## Steps

Step-1: Firstly we have to connect to the machine we are attacking using the `ssh user@userIP` command and then enter the password of the user.

<img width="784" height="391" alt="Screenshot 2026-02-11 161041" src="https://github.com/user-attachments/assets/80708ece-1957-4775-8e99-9b1da81edd06" />

<br><br>

Step-2: After enter the password (given in the task which is “tryhackme”) we will see something like this:

<img width="796" height="486" alt="Screenshot 2026-02-11 161327" src="https://github.com/user-attachments/assets/e7020bfa-47e5-4ce5-a7c6-e6bec204e115" />

<br><br>

Step-3: Now our goal is to download the flag.txt from the remote pc (tryhackme) by running the server.

<img width="732" height="168" alt="Screenshot 2026-02-11 164323" src="https://github.com/user-attachments/assets/ffd9cbdf-a40b-4a53-86aa-c77f34adf93d" />

<br><br>

Step-4: Then we just have to download the file using the `wget sourceaddress` command.

<img width="905" height="290" alt="Screenshot 2026-02-11 164501" src="https://github.com/user-attachments/assets/7628e4b8-bc9b-4975-b6fa-262901ad19ee" />

<br><br>

Step-5: Now that we have the file in our pc, we can easily check the content of the file. Since it is a .txt file we can print all data from it using the `cat filename` command.

<img width="924" height="371" alt="Screenshot 2026-02-11 164758" src="https://github.com/user-attachments/assets/59c4a168-49fb-46c5-af77-b89622b6d698" />

<br><br>

> Flag found: THM{WGET_WEVSERVER}

<br><br>

---
---

<br><br>

# <p align="center"> Room: Linux fundamentals part 3, task-8 </p>
---

## Objective: getting IP address of a user from log file

## Tool used: nano (for log file reading), ssh (for connecting to THM machine)

## Steps

Step-1: Connect to the remote machine using the “ssh user@userIP” command.

<img width="646" height="510" alt="Screenshot 2026-02-11 234807" src="https://github.com/user-attachments/assets/435cf7d2-5071-43e2-8e26-e3cfb09d0d27" />

<br><br>

Step-2: go to the logs folder using “cd” and “ls” commands.

<img width="1051" height="515" alt="Screenshot 2026-02-11 235029" src="https://github.com/user-attachments/assets/94bacb92-2a8e-466d-8189-033b7b8c2244" />

<br><br>

Here we can see all types of .log files. Our goal is to find out the IP of a user who visited a site. So we can find that log inside the “apache2” folder. 

<img width="782" height="166" alt="Screenshot 2026-02-11 235430" src="https://github.com/user-attachments/assets/57504fe9-2a87-454c-b568-1608946d6450" />

<br><br>

Step-3: Inside the apache2 folder we have permission to read “access.log.1” and “error.log.2.gz” . In that case we will try to read both of these files to check if we get some info. We will use nano for that.

<img width="1718" height="325" alt="Screenshot 2026-02-12 000205" src="https://github.com/user-attachments/assets/437722b5-0f8e-4d56-9242-102608af217c" />

<br><br>

> IP: 10.9.232.111
> File tried to access: catsanddogs.jpg

<br><br>

---
---
