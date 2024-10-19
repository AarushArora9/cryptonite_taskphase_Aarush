# Hello
## Challenge 1: Chaining with semicolons
In this challenge I had to chain two commands to get the flag
### Method
To do so I used the ```;``` operator which helped me chain the commands ```/challenge/pwn``` and ```/challenge/college``` the final command being ```/challenge/pwn; /challenge/college``` which 
gave me the flag:
```pwn.college{kb_pKcni38i80taXpLhX5FH2T4q.dVTN4QDLxkDN1czW}```
## Challenge 2: Your First Shell Script
In this challenge I had to create a shell file, write the required commands in the shell file and then execute the commands from the shell file
### Method
I first created the required file using the command ```touch x.sh``` and then I wrote the required commands in the file using the command ```echo "/challenge/pwn; /challenge/college"> x.sh```
and then executed the shell files using the command ```bash x.sh``` to get the flag:
```pwn.college{sz4l5xXxBELVAO8PFt169ROGxV9.dFzN4QDLxkDN1czW}```
## Challenge 3: Redirecting Script Output
In this challenge I had to pipe the output of a shell file into another command
### Method
To do so I first created a shell file using the command ```touch script.sh``` Then I wrote the required commands in the shell file using the command
```echo "/challenge/pwn; /challenge/college"> x.sh``` then I piped the output of this shell file to ```/challenge/solve``` using the command ```bash script.sh | /challenge/solve```
which gave me the following flag
```pwn.college{Qdw2r3R2uSlcDF7_gK4BbjgZNfo.dhTM5QDLxkDN1czW}```
## Challenge 4: Executable Shell Scripts
In this challenge I had to run the shell file with a specified command after making it executable and invoke the shell file without using ```bash```
### Method
To do so I first made a shell file using the command ```touch script.sh``` then I wrote the specified command in the file using the command ```echo "/challenge/solve">script.sh```
then I made the file executable using the command ```chmod u=rwx script.sh``` and then I ran it using the command ```./script.sh``` which gave me the flag
```pwn.college{cG0-qZ3_puISQ-j5LlfhirtnAFY.dRzNyUDLxkDN1czW}```
