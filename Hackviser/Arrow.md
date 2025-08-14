# Q1: Which Ports are Open
I used the following command to find the open ports:

nmap 172.20.13.127


<img width="519" height="118" alt="image" src="https://github.com/user-attachments/assets/6f700c5f-25bc-40e4-9ea9-3cae3fb13775" />


# Q2: What is the running service name?
After doing the nmap scanning for the first question. 

I was able to find the answer "telnet" for this question.

<img width="519" height="118" alt="image" src="https://github.com/user-attachments/assets/96de1696-0fee-440f-9455-537b67bccd4a" />


# Q3: What is the hostname?
To find the hostname. I tried to connect the machine using the following command:

telnet 172.20.13.127

After that I used the "hostname" command.

<img width="183" height="32" alt="image" src="https://github.com/user-attachments/assets/f55587c9-f485-4c76-a8c6-3d2ab38be210" />


# Q4: What is the working directory location when you connect to telnet?
I used the "pwd" command.

<img width="144" height="31" alt="image" src="https://github.com/user-attachments/assets/2b8acb93-03b8-4e12-9757-e41eb9d7807c" />
