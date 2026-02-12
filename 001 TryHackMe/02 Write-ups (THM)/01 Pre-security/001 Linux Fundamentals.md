# <p align="center"> Room: Linux Fundamentals part 3 / Task-4 </p>

## Objective: connecting to a pc remotely and flag capturing

## Command used: `ssh`, `cd`, `ls`, `scp`, `wget`

## Steps

1. Firstly we have to connect to the machine we are attacking using the `ssh user@userIP` command and then enter the password of the user.

<img width="784" height="391" alt="Screenshot 2026-02-11 161041" src="https://github.com/user-attachments/assets/80708ece-1957-4775-8e99-9b1da81edd06" />

<br><br>

2. After enter the password (given in the task which is “tryhackme”) we will see something like this:

<img width="796" height="486" alt="Screenshot 2026-02-11 161327" src="https://github.com/user-attachments/assets/e7020bfa-47e5-4ce5-a7c6-e6bec204e115" />

<br><br>

3. Now our goal is to download the flag.txt from the remote pc (tryhackme) by running the server.

<img width="732" height="168" alt="Screenshot 2026-02-11 164323" src="https://github.com/user-attachments/assets/ffd9cbdf-a40b-4a53-86aa-c77f34adf93d" />

<br><br>

4. Then we just have to download the file using the `wget sourceaddress` command.

<img width="905" height="290" alt="Screenshot 2026-02-11 164501" src="https://github.com/user-attachments/assets/7628e4b8-bc9b-4975-b6fa-262901ad19ee" />

<br><br>

5. Now that we have the file in our pc, we can easily check the content of the file. Since it is a .txt file we can print all data from it using the `cat filename` command.

<img width="924" height="371" alt="Screenshot 2026-02-11 164758" src="https://github.com/user-attachments/assets/59c4a168-49fb-46c5-af77-b89622b6d698" />

<br><br>

> Flag found: THM{WGET_WEVSERVER}
<br><br>
---
