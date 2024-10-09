# HELLO
## Challenge 1: Redirecting output
In this challenge, I had to write the string "PWN" to the file ```COLLEGE``` using the command ```echo```
### Method
I ran the command ```echo PWN > COLLEGE``` to write the string to the aforementioned and got the flag
```pwn.college{UtA-uoVTYiG5EW9Hd4JFMF0xr23.dRjN1QDLxkDN1czW}```
## Challenge 2: Redirecting more output
In this challenge I had to redirect the out of ```/challenge/run``` to the file ```myflag```
### Method
To do that I used the command ```/challenge/run > myflag``` which redirected the the flag to the file and I read the file using ```cat myflag``` to get the flag
```pwn.college{g3W7Rk-evYlONpeTeGDLCkeKby6.dVjN1QDLxkDN1czW}```
## Challenge 3: Appending Output
In this challenge, I had to append the output of the command ```/challenge/run``` to the file ```home/hacker/the-flag``` using the append mode
### Method
I did so by executing the command in append mode as in ```/challenge/run >> /home/hacker/the-flag``` which appended the first half of the flag to the last one
and I read the file and got the flag by using the command ```cat /home/hacker/the-flag```, the flag being ```pwn.college{EoYJJH7YrCPj9Be79TJUVPulxED.ddDM5QDLxkDN1czW}```
## Challenge 4: Redirecting errors
In this challenge, I had to redirect the out of ```/challenge/run``` to the file ```myflag``` but the errors to the file ```instructions```
### Method
I used the File Descriptor Numbers to achieve the goal of the challenge because I can use them to redirect the files appropriately using them before > character while redirecting
I ran the command ```/challenge/run > myflag 2> instructions``` to achieve the goal of the challenge and then I got the flag by printing the contents of the file ```myflag``` using the c
```cat``` command, the overall command being ```cat myflag``` which gave me the flag ```pwn.college{spEMq5B4_qMs1PsijCcxY9sFpwY.ddjN1QDLxkDN1czW}```
## Challenge 5: Redirecting Input
In this challenge I had to redirect the file ```PWN``` containing the value ```COLLEGE``` to the command ```/challenge/run```
### Method
I first ran the command ```echo COLLEGE > PWN``` to store the value in the file and then used the command ```/challenge/run < PWN``` to redirect the file ```PWN``` to ```/challenge/run```
and I got the flag  ```pwn.college{gsQBaA9yhAx-qnQe77qcbpdDOnY.dBzN1QDLxkDN1czW}```
## Challenge 6: Grepping stored results
In this challenge, I had to grep the flag after storing the output of a command in a text file
### Method
I first ran the command ```/challenge/run > /tmp/data.txt``` to store the output of command ```challenge/run``` in the specified text file ```data.txt```
since the flag always starts with ```pwn.college``` the grepped the flag out of the file using the command ```grep 'pwn.college' /tmp/data.txt``` to get the flag
```pwn.college{IXh5ddEDZ4JUYYlqjLkdWfLAG8r.dhTM4QDLxkDN1czW}```
## Challenge 7: Grepping Live Output
In this challenge I had to directly grep the flag from the output of comamnd ```/challenge/run``` 
### Method
I used the pipe operator ```|``` for this so that output of the command ```/challenge/run``` is directly used as input for grep
I used the grep command with the search string ```pwn.college``` because every flag has that string
This gave me the overall command as ```/challenge/run | grep 'pwn.college'``` and gave me the flag
```pwn.college{YBnnRElYKmCYlsv12xUW83PuBIy.dlTM4QDLxkDN1czW}```
## Challenge 8: Grepping errors
In this challenge I had to grep the errors to get the flag 
### Method
I had to use ```>&``` operator which directs one file descriptor to another, using which I can direct errors to standard output using this in addition to the pipe operator
```|``` to direct the output of the first command to input of the second one, which gives the overall command as
```/challenge/run 2>&1| grep 'pwn.college'``` exceuting which gives us the flag
```pwn.college{Uf9eHZN0IouGgqtLyUHVU2mnay-.dVDM5QDLxkDN1czW}```
## Challenge 9: Duplicating piped data with tee 
In this challenge I had to ```tee``` command to intercept the command to reach the flag
### Method
I first executed the command ```/challenge/pwn | tee i.txt | /challenge/college```  which intercept the command /challenge/pwn and stored its output in the file i.txt which on reading with
the ```cat``` command reveals that I need to use the argument ```--secret [SECRET_ARG]``` the secret argument being "slEGhqoh" so this time I executed the command again with proper arguments
```/challnege/pwn --secret slEGhqoh | /challenge/college``` which gave me the ```flag pwn.college{slEGhqoht2Q_bOy2xwL8DhwFVez.dFjM5QDLxkDN1czW}```
## Challenge 10: Writing to multiple programs
In this challenge I had to redirect the output of one command into two different commands using the pipe operator
### Method
To do so I piped the output of ```/challenge/hack``` to ```/challenge/the``` and ```/challenge/planet``` as required using the command 
```/challenge/hack | tee >( /challenge/the ) >( /challenge/planet )``` which gave me the required flag as
```pwn.college{4BCGudZ5hFlkweE3PC2MBjUx6U-.dBDO0UDLxkDN1czW}```
## Challenge 11: Splitt-piping stderr and stdout
In this challenge I had to redirect the stdout and stderr of command ```/challenge/hack``` to ```/challenge/planet``` and ```/challenge/the``` respectively
### Method
To do so I first used the command ```/challenge/hack > 2> >(/challenge/the) >(/challenge/planet)``` but it gave me an error because it was not able to identify ```2``` as a File Descriptor 
and gave the ```unexpected token error``` to fix this I switched the order in the command so that first it starts redirecting the stdout and is able to identify the File Descriptor
which gave me the overall command ```/challenge/hack > >(/challenge/planet) 2> >(/challenge/the)``` which gave me the required flag as
```pwn.college{0M_LD93egotXjlJw040Xj-3Y4Y0.dFDNwYDLxkDN1czW}```

