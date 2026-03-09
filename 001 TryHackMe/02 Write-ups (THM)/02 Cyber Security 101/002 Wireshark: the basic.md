# <p align="center">Room: Wireshark: The basics / Task-4</p>
---
### Overview: 
In this task we will follow the instructions given in the question and capture the flag. This will improve our wireshark navigating skills. We will use the tool wireshark for that and use various function of it like find packet, go to packet, export object etc.

---

# Obj-1: finding hash by navigating the packet

### Question: 
Go to packet 12 and read the packet comments. What is the answer?<br>
Note: use md5sum <filename> terminal command to get MD5 hash<br>

### Step-1: go the the packet 12 using "go to" function from the toolbar
<img width="1903" height="863" alt="image" src="https://github.com/user-attachments/assets/ece91946-f3dd-4c5e-8134-827bab73a712" />
here we can see they gave us more instructions to follow <br>

### Step-2: as instructed, we are going to the packet number 39,756 using "go to"
<img width="1909" height="864" alt="image" src="https://github.com/user-attachments/assets/9dda363a-0fa3-4241-8921-7d7f765ed85a" /><br>

### Step-3: in the packet information, we can see theres a JPEG layer. we have to export packet byte and save it using any name in any location. I am saving it as "task-4" in the documents directory
<img width="1897" height="864" alt="image" src="https://github.com/user-attachments/assets/7b9d90c8-9af1-45c8-8f83-986be632477e" />
<img width="1895" height="864" alt="image" src="https://github.com/user-attachments/assets/de3fc4a1-e147-48fd-9cf7-09b4705162d2" />
We are done with the packet in wireshark, now we have to get the hash using the command ```md5sum filename```<br>

### Step-4: open terminal and browse to the file we exported earlier and get the hash using given command.
<img width="910" height="662" alt="image" src="https://github.com/user-attachments/assets/59c736a5-15a0-49d8-ad23-b48e83700d85" />

---
<br>

### Hash: 911cd574a42865a956ccde2d04495ebf

<br>

---

# Obj-2: Reading a text from the packet using the skills we learned

### Question: 
There is a ".txt" file inside the capture file. Find the file and read it; what is the alien's name? <br>

### Step-1: since we are finding a text file in the captured packet, we will use the find function or ctrl+f to search the packet with txt file 
<img width="1892" height="860" alt="image" src="https://github.com/user-attachments/assets/f2102d89-4bb1-4004-bb8a-9027b2a6f3e9" />
here we found the packet with text file<br>

### Step-2: view details of the packet by double-clicking it and scroll down for the content
<img width="1897" height="858" alt="image" src="https://github.com/user-attachments/assets/11a890ec-1696-4ff3-af02-1906a9e4c7d0" /><br>

---
### Alien name: PACKETMASTER







