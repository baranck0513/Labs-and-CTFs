# Q1: Which port(s) are open?
I used the following command:

```bash
nmap 172.20.8.90
```

However, the machine did not let me see the open ports because they were filtered:

<img width="672" height="96" alt="image" src="https://github.com/user-attachments/assets/fb5b137c-c103-42b2-b0e5-58716a5c0bd4" />

So, I come up with different approach:

```bash
nmap -p- -sT -v 172.20.8.90
```

- "-p-" for scanning all of the ports 
- "-sT" for TCP connect scan
- "-v" for more verbose output

<img width="704" height="305" alt="image" src="https://github.com/user-attachments/assets/f64d48c0-dfa5-4396-9b02-a1da589452f1" />

# Q2: What is the version number of the running Redis service?

In order to determine the version number, I used the following:

```bash
nmap -p 6379 -sT -v -sV 172.20.8.90
```

- "-sV" parameter in Nmap adds service version detection to the scan process

<img width="527" height="47" alt="image" src="https://github.com/user-attachments/assets/bc25c45e-cb23-4060-9335-9f22c2ed95a9" />

# Q3: How many key-value pairs are there?

I used the following command to establish a connection to Reddis server:

```bash
redis-cli -h 172.20.8.90 -p 6379
```

Then I used:

```bash
keys *
```

to find the all key-value pairs

# Q4: What is admin's sessionToken value?

<img width="246" height="229" alt="image" src="https://github.com/user-attachments/assets/1c6b359d-f700-40de-bd1f-14239982f31b" />


<img width="1117" height="98" alt="image" src="https://github.com/user-attachments/assets/dcac5ba5-4e3f-489a-82b8-e8fc8bf8e303" />
