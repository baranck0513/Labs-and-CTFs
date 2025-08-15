# Q1: Which port(s) are open?

I used the following command to find the open ports:

```bash
nmap 172.20.3.19
```

# Q2: What username did you connect to the FTP?

I connected to the FTP server using:

```bash
ftp 172.20.3.19
```

Then I saw I can login with the anonymous account without needing to enter the password.

<img width="483" height="95" alt="image" src="https://github.com/user-attachments/assets/609f6e0c-e718-4077-9c67-f5e2598f89d3" />

# Q3: What is the name of the file on the FTP server?

After logging in, I used the "ls -la" command to list all the files in the server.

<img width="655" height="121" alt="image" src="https://github.com/user-attachments/assets/92785445-2ebd-4e59-8627-31fd7c7e8cda" />

Then I saw there is a file named "userlist"

# Q4: Which users' information is in the file?

In order to read the information in that file. I downloaded that file into my own machine using:

```bash
get userlist
```

<img width="657" height="115" alt="image" src="https://github.com/user-attachments/assets/2e5db232-b983-4fc2-9b76-fd707021d398" />

After, I used the following:

<img width="215" height="57" alt="image" src="https://github.com/user-attachments/assets/bb8eb702-0e5b-4c8b-aaa2-92b5f6e6249f" />
