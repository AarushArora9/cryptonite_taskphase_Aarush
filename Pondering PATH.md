# Hello
## Challenge 1: The PATH variable
In this challenge I had to change the value of the shell variable and then invoke a command to get the flag
### Method
To prevent the deletion of the flag I set the shell variable to store nothing using the command ```PATH=""``` then I executed the command ```/challenge/run```
which gave me the flag:
```pwn.college{I_t5MUNYjZWHMdmhyxMwM3wH-sO.dZzNwUDLxkDN1czW}```
## Challenge 2: Setting PATH
In this challenge I had set the shell variable with a certain path to get the flag
### Method
To do so I set the shell variable to the required path ```/challenge/more_commands/``` using the command ```PATH="/challenge/more_commands/"``` and the I ran the command ```/challenge/run``` to
get the flag:
```pwn.college{sEWZZFA8sNNtI1IYlxw31q7yGiv.dVzNyUDLxkDN1czW}```
## Challenge 3: Adding Commands
In this challenge I had to create a custom shell script that would allow a command to retrieve a flag
### Method
To do so I first created a file name ```win``` using the command ```touch win``` then I put the command to retrieve the flag ```cat /flag``` inside the file using the command 
```echo "cat /flag"> /home/hacker/win``` then to allow the command ```/challenge/run``` to find the ```win``` script I added the directory containing ```win``` to the PATH using the command 
```PATH=PATH$:/home/hacker``` then I changed the permissions of the script ```win``` to make it executable using the command ``` chmod a+x /home/hacker/win``` then I executed the command
```/challenge/run``` to get the flag:
```pwn.college{0XL2pQEAzw-xA5YEYi8bQBGjcG3.dZzNyUDLxkDN1czW}```
## Challenge 4: Hijacking commands
In this challenge I had to hijack the ```rm``` script and change it so that the flag is displayed
### Method
To do so I first created a script in the home directory using the command ```touch rm``` then I wrote the command into the script which will get the flag using the command 
```echo "cat /flag">/home/hacker/rm``` then I changed the file permissions to make it executable using the command ```chmod a+x /home/hacker/rm``` I then updated the path so that my custom
script ```rm``` is used and not the system one using the command, ```PATH=/home/hacker/$:PATH``` then I executed the command ```/challenge/run``` to get the flag which was:
```pwn.college{khj4Lvy2cz8fc9hlm3eOnwsLoZD.ddzNyUDLxkDN1czW}```
