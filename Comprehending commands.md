# Hello 
## Challenge 1: cat : not the pet but the command
In this challenge, I had to use the cat command to copy the flag to the flag file in the home directory
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
In this challenge, I had to cat the file hidden in a directory
### Method
The directory in which the flag was hidden was told to be ```/lib/dpkg``` directory
I used the command ```cat /lib/dpkg/glag``` to cat the file which resulted in the following flag
```pwn.college{ghCcuBVdH0hY4q2Diarca0x0S8f.dBjM5QDLxkDN1czW}```
## Challenge 4: grepping for a needle in a haystack
In this challenge, I had to grab the flag from a file stored in /challenge/data.txt
### Method 
I used the ```grep``` command with the ```SEARCH_STRING``` as ```pwn.college``` which provided the following flag required to complete the challenge
```pwn.college{Mw4T1QhOzQJeKRj8gLwMz47pvQb.ddTM4QDLxkDN1czW}```
## Challenge 5: listing files
In this challenge, I had to use the ```ls``` command to locate the flag file inside the ```/challenge``` directory which has been renamed 
### Method 
I used the ```ls /challenge``` command to list all the files inside ```/challenge``` which gave me the name of the renamed file as
```20509-renamed-run-2178.md``` which I accessed and read from the home directory using ```/challenge/20509-renamed-run-21768 DESCRIPTION.md```
and got the flag ```pwn.college{4UIyRah-XazpvdbuoqlWepOsM2k.dhjM4QDLxkDN1czW``` required.
## Challenge 6: touching files 
In this challenge, I had to create files using the touch command
### Method
To do so I first changed my directory to the required directory using the command ```/cd tmp``` then I used the ```touch``` command to create the do files using 
the command ```touch pwn``` and ```touch college``` to create the required files and then used the ```challenge/run``` command to get the required flag which was 
```pwn.college{0L_kHL7ZnFJxulv9T4trlLKifYM.dBzM4QDLxkDN1czW}```
## Challenge 7: removing files 
In this challenge, I had to delete a file using the ```rm``` command
### Method
I first created the file in some directory using the command ```touch delete_me``` then I deleted it using the command ```rm delete_me``` and then ran the command
```/challenge/check``` to get the following flag required to complete the challenge
```pwn.college{43srr13Jf-q1l7Ue7Gc-GHp2gIp.dZTOwUDLxkDN1czW}```
## Challenge 8: hidden files
In this challenge, I had to view the hidden files using the ```-a``` prompt with the ```ls``` command
### Method
I first used the ``` cd /``` command to change the working directory to the root directory then I used the ```ls ``` command flag ```-a``` to view all the files
among which the file containing flag was ```.flag-10892314262974``` which I cat using command ``` cat /.flag-10892314262974``` to get the mentioned flag 
```pwn.college{QPkaNBAwnIOAFnLegCtFRXf0TOS.dBTN4QDLxkDN1czW}```
## Challenge 9: An Epic Filesystem Quest
In this challenge, I had to implement the knowledge of basic Linux commands to navigate a file system and find a hidden flag.
### Method
This challenge was an epic journey of failure, success, frustration, anger, perseverance, and most importantly navigating the maze of file directories. The journey started by changing the working directory to the root directory using ```cd /``` then came the use of ```ls``` to view the files in the director, upon doing so ```SPOILER``` file was discovered which was cat to display its contents using ```cat SPOILER```
the next clue was thus discovered and the directory was changed accordingly to access its contents, then we stumbled upon another clue this time the clue was hidden so ```ls -a``` command had to be used to reveal it. When the next clue was revealed it was found that the directory mentioned in the clue can only be accessed without using ```cd``` command else the clue will self distruct. These challenges lasted for a while until the final clue and file path ```opt/aflplusplus/nyx_mode/QEMU-Nyx/pc-bios/keymaps/.BLUEPRINT``` and the
flag was accessed
```pwn.college{UVqUuPkmjhE753pZ2jVT7xXzvZ9.dljM4QDLxkDN1czW}```
## Challenge 10: making directories
In this task we had to use the ```mkdir``` command 
### Method
I first changed my directory to required ```tmp``` directory using the ```cd /tmp``` command and than I used the command to make a directory there ```mkdir pwn``` and the required file ```touch pwn/college```, then I execute the ```/challenge/run``` command to get the final flag which was ```pwn.college{QEHepc9_qQ0zP-lcu16193hed_5.dFzM4QDLxkDN1czW}```
## Challenge 11: finding files
In this task I had to find the file containing the flag using the ```find``` command
### Method 
I used the ```find / -name flag``` command to find all the instances of the file/directory flag in the file system and then I sifted through
them manually to find the required flag which was ```pwn.college{EP-3A9IEZxPo6ZLsX-LAihP5jyE.dJzM4QDLxkDN1czW}```
## Challenge 12: linking files
In this challenge I have to soft link two files to get the flag using the ```ln -s``` command
### Method
I first change my directory to the root directory using ```cd /``` then link the ```/flag``` file to the ```/home/hacker/not-the-flag``` file using the command ```ln -s /flag /home/hacker/not-the-flag``` then I access ```/challenge/catflag``` file which gives me the required flag
```pwn.college{cKPzXVT3yFoqj4q-PbmzZVogRIS.dlTM1UDLxkDN1czW}```
