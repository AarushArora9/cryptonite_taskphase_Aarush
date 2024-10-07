# Hello 
## Challenge 1: cat : not the pet but the command
In this challenge I had to use the cat command to copy the flag to the flag file in the home directory
### Method
I used the command ```cat flag``` which displayed the contents of the file and provided the flag
```pwn.college{MTORG8eqqmaisFT1OXbmkqhNf0M.dFzN1QDLxkDN1czW}```
## Challenge 2: catting absolute paths
In this challenge I had to make the flag file readable
### Method
I did so using the 
```car /flag``` command which gave me the flag
```pwn.college{I_dunfZ-vjCOlaqwZLE11u3yXT1.dlTM5QDLxkDN1czW}```
## Challenge 3: more catting practice
In this challenge I had to cat the file hidden in a directory
### Method
The directory in which the flag was hidden was told to be ```/lib/dpkg``` directory
I used the command ```cat /lib/dpkg/glag``` to cat the file which resulted in the following flag
```pwn.college{ghCcuBVdH0hY4q2Diarca0x0S8f.dBjM5QDLxkDN1czW}```
## Challenge 4: grepping for a meedle in a haystack
In this challenge I had to grab the flag from a file stored in /challenge/data.txt
### Method 
I used the ```grep``` command with the ```SEARCH_STRING``` as ```pwn.college``` which provided with the following flag required to complete the challenge
```pwn.college{Mw4T1QhOzQJeKRj8gLwMz47pvQb.ddTM4QDLxkDN1czW}```
## Challenge 5: listing files
In this challenge I had to use the ```ls``` command to locate the file inside ```/challenge``` directory which has been renamed 
### Method 
I used the ```ls /challenge``` comamnd to list all the files inside ```/challenge``` which gave me the name of the renamed file as
```20509-renamed-run-2178.md``` which I accessed and read from the home directory using ```/challenge/20509-renamed-run-21768 DESCRIPTION.md```
and got the flag ```pwn.college{4UIyRah-XazpvdbuoqlWepOsM2k.dhjM4QDLxkDN1czW``` required.
## Challenge 6: touching files 
In this challenge I had to create files using the touch command
### Method
To do so I first changed my directory to the required directory using the command ```/cd tmp``` then I used the ```touch``` command to create the do files using 
the command ```touch pwn``` and ```touch college``` to create the required files and then used the ```challenge/run``` command to get the required flag which was 
```pwn.college{0L_kHL7ZnFJxulv9T4trlLKifYM.dBzM4QDLxkDN1czW}```
## Challenge 7: removing files 
In this challenge I had to delete a file using the ```rm``` command
### Method
I first created the file in fome directory using the command ```touch delete_me``` then I deleted it using the command ```rm delete_me``` and then ran the command
```/challenge/check``` to get the following flag required to complete the challenge
```pwn.college{43srr13Jf-q1l7Ue7Gc-GHp2gIp.dZTOwUDLxkDN1czW}```
## Challenge 8: hidden files
In this challenge I had to view the hidden files using the ```-a``` prompt with the ```ls``` command
### Method
I first used the ```cd /1``` command to change change the working directory to the root directory then I used the ```ls ``` command flag ```-a``` to view all the files
among which the file containting flag was ```.flag-10892314262974``` which I cat using command ``` cat /.flag-10892314262974``` to get the mentioned flag
```pwn.college{QPkaNBAwnIOAFnLegCtFRXf0TOS.dBTN4QDLxkDN1czW}```
## Challenge 9: An Epic Filesystem Quest
In this challenge I had to implement the knowledge of basic Linux commands to navigate a filesystema and find a hidden flag.
### Method
