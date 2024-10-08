# Hello
## Challenge 1: Matching with *
IN this challenge I had to use the glob ```*``` to change my directory to ```/challenge``` using at most 4 characters
### Method
I did so by running the command ```cd /c*``` which changed my directory to ```/challenge``` because the glob ```*``` treats any argument like a 
wildcard and searches for all possible combinations which in this case was ```/challenge```, then I ran the ```/challenge/run``` command to 
get the required flag which was ```pwn.college{chel9WJ2tEgVwxbBUJUUb9_iryY.dFjM4QDLxkDN1czW}```
## Challenge 2: Matching with ?
In this challenge I had to use the glob ```?``` to change my directory to ```/challenge```
### Method
Since glob ```?``` works similarly to ```*``` but only searches for single characters I used the glob 9 times (length of the word challenge)
to change the directory as required by running the command ```cd /*********``` and then accessed the flag using the command ```/challenge/run```
which gave me the flag ```pwn.college{AL35sN7Ka74cb3VVzuV2zpzNwE7.dJjM4QDLxkDN1czW}```
## Challenge 3: Matching with []
In this challenge I had to use the glob ```[]``` for finding the flag
### Method
I first changed my directory to ```/challenge/files``` using the command ```cd /challenge/files``` then I ran the command ```/challenge/run```
with the bracket-globs ```files_[bash]``` to get the required flag which was ```pwn.college{sZ32DBXWT5Feec7b5f9lXnChCAY.dNjM4QDLxkDN1czW}```
## Challenge 4: Matching paths with []
In this challenge I had to run a single argument of bracket-globs of file stored in ```/challenge/files``` from my home directory
### Method
I did so by running the ```/challenge/run``` command with the arguments ```/challenge/files/file_[bash]``` which use the absolute path of the 
files stored in ```/challenge/files``` with a single bracket-glob ```file_[bash]``` using the overall command 
```/challenge/run /challenge/files/file_[bash]``` to get the required flag
```pwn.college{Y06PT5VhZI7q6Z1PkGab2-uYL7e.dRjM4QDLxkDN1czW}```
## Challenge 5: Mixing Globs
In this challenge I had to mix the globs to match the files "challening", "educational", and "pwning"
### Method
I first changed my directory to ```/challenge/files``` as instructed in the challenge description using the command ```cd /challenge/files```
then to match the files I had to run the command ```/challenge/run``` with a glob suitable for finding all the files, since letters c, e and p
were unique to each I used the bracket glob ```[cep]*``` where the glob ```*``` serves the purpose of searching through all possible 
combinations, I finally ran the overall command ```/challenge/run [cep]8``` to get the required flag 
```pwn.college{4DNiMv-YTQcrJdZj2XDFvRI4Ri4.dVjM4QDLxkDN1czW}```
## Challenge 6: Exclusionary globbing
In this challenge I had to match all the files that didnt' start with p, w or n
### Method
I first changed my directory to ```/challenge/files``` as instructed in the challenge description using the command ```cd /challenge/files```
then to match all the files that doesn't start with p, w or n I used the bracket-glob ```[^pwn]8``` with glob ```*``` serves the purpose of 
going through all the possible combinations, I finnally used the glob with the command ```/challenge/run``` go give the overall command
```/challenge/run [^pwn]*``` to get the required flag as ```pwn.college{km7qvqFGwqy-EgcHlCAOhcl_XbL.dZjM4QDLxkDN1czW}```
