# Hello
## Challenge 1: Changing File Ownership
In this challenge I had to change ownership of a file
### Method
I did so using the ```chown``` command and specifying the new user and the file name, the overall command was ```chown hacker /flag``` and then I read the file using the command ```cat /flag``` which gave me the flag
```pwn.college{83Drc2UDVUQYf806uerbGdgSKjt.dFTM2QDLxkDN1czW}```
## Challenge 2: Groups and Files
In this challenge I had to change the group of a file to get the flag
### Method
I used the ```chown``` command to do so by specifying the new user and file name, the overall command being ```chgrp hacker /flag``` Then I read the file using the command ```cat /flag``` to get the flag which was
```pwn.college{w7uNuYLPEw--1iYo8DU7rpethdd.dFzNyUDLxkDN1czW}```
## Challenge 3: Fun with Groups Names
In this challenge I had to change the group of the file to the correct group to get the flag
### Method
I used the ```id``` command to get the group name which was ```grp14241``` so I changed the group of the file to the same using the command ```chgrp grp14241 /flag``` and then read the file using the command
```cat /flag``` to get the flag which was  ```pwn.college{c5ou7wX_mgoYB73XBw-dOGRNXyv.dJzNyUDLxkDN1czW}```
## Challenge 4: Changing Permissions
In this challenge I had to change the permission of the file to access it and get the flag
### Method 
I did so using the command ```chmod``` and the appropriate arguments which were ```go+rwx``` which allows the user and other users to read, modify, and execute the file, which gave me the command as 
```chmod go+rwx /flag```, I read the flag and I got the flag as ```pwn.college{Uf9cQIW7ucJAzhJvi_OT47tEwgC.dNzNyUDLxkDN1czW}```
## Challenge 5: Executable Files
In this challenge I had to change the permission of the executable ```/challenge/run```
### Method
I used the ```chmod``` command to change the user permissions and allowed the user to run the file using the command ```chmod u+x /challenge/run``` and then I executed the file using the command ```/challenge/run```
to get the flag ```pwn.college{4ylsOTh38dJgfatIkx8QwOiKlB5.dJTM2QDLxkDN1czW}```
## Challenge 6: Permission Tweaking Practice
In this challenge I had to solve several challenges to get the opportunity to change the permissions of the flag file and read it to get the flag
### Method
I first ran the ```/challenge/run``` command which gave me instructions according to which I changed the permissions of the file ```/challenge/run```, the commands I used for changing the permissions were:
``` chmod u+x /challenge/pwn```
``` chmod g-r /challenge/pwn```
``` chmod o+x /challenge/pwn```
``` chmod o-rx /challenge/pwn```
``` chmod g+wx /challenge/pwn```
``` chmod ug-rwx /challenge/pwn```
``` chmod u+rx /challenge/pwn```
``` chmod u-x /challenge/pwn```
then I changed the permissions of the file ```/flag``` using the command ```chmod ugo+rwx /flag``` and read its contents to get the flag using the command ```cat /flag``` which gave me the following flag
```pwn.college{s_Yne0pOZYhu5V-l2A9Kfe4AD4S.dBTM2QDLxkDN1czW}```
## Challenge 7: Permission setting practice
In this challenge, I had to solve 8 challenges to change the permission of file ```/flag``` and get the flag
### Method
I first ran the command ``/challenge/run`` which instructed me to change the permissions of the file ```/flag``` for which I had to use the ```=``` and ```,``` argument in command ```chmod``` to change the 
permissions of the file ```/challenge/pwn``` as follows
```chmod u=-,g=-,o=x /challenge/pwn```
```chmod u=w,g=rx,o=rw /challenge/pwn```
```chmod u=rw,g=-,o=w /challenge/pwn```
```chmod u=rx,g=rw,o=wx /challenge/pwn```
```chmod u=r,g=rwx,o=rx /challenge/pwn```
```chmod u=w,g=w,o=w /challenge/pwn```
```chmod u=w,g=rx,o=wx /challenge/pwn```
```chmod u=rwx,g=wx,o=rw /challenge/pwn```
then I changed the permissions of the file ```/flag``` using the command ```chmod ugo+rwx /flag``` and read its contents to get the flag using the command ```cat /flag``` which gave me the following flag
```pwn.college{8XGXMu_uktIh9UvLIjC4M8yyUyB.dNTM5QDLxkDN1czW}```

## Challenge 8: The SUID Bit
In this challenge, I had to add SUID bit to the program ```/challenge/getroot``` and get access to the root shell to get the flag
### Method 
I did so by executing the command ```chmod u+s /challenge/getroot``` which set the SUID bit of the file, then I executed the file using the command ```/challenge/getroot``` which gave me access to the root shell
and allowed me to use the command ```cat /flag``` to get the flag, which was ```pwn.college{ATl1zIVOjuZoyiRzNZ852BZOWKs.dNTM2QDLxkDN1czW}```
