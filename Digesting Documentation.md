### Hello
## Challenge 1: Learning from documentation
In this challenge, we had to capture the flag using the proper arguments of the file
### Method
To solve this challenge I executed the command to access the file ```/challenge/challenge/``` with the proper required argument ```--giveflag```
appended to it like so : ```/challenge/challenge --giveflag``` to get the required flag
```pwn.college{cE8HBmcJQay6zabA9ZpqmAFHgXk.dRjM5QDLxkDN1czW}```
## Challenge 2: Learning Complex Usage
In this challenge, I had to use the correct argument to access the file and capture the flag
### Method
In this challenge the flag was stored in the ```/flag``` file in the ```/challenge/challenge``` directory so I used the argument ```--printfile```
to access the file using the command ```/challenge/challenge --printfile /flag``` to capture the required flag
```pwn.college{48AV5G-ee0Y7WnUExFfR6TflOAk.dVjM5QDLxkDN1czW}```
## Challenge 3: Reading Manuals 
In this challenge, I had to use the ```man``` command to read the manual and get the institutions to capture the flag
### Method
I first ran the command ```man challenge``` which gave me the information I needed to access```/challenge/challenge``` directory with the 
argument ```--gjjhod 801``` to access the flag, to do so I ran the command ```/challenge/challenge --gjjhod 801``` which gave me the 
required flag ```pwn.college{gSj80jTHJho-Ddqxb1uHWx8_XYd.dRTM4QDLxkDN1czW}```
## Challenge 4: Searching Manuals
In this challenge, I had to search a manual using the ```/``` command and the appropriate search term
### Method
I first ran the command ```man challenge``` to access the challenge manual which had a lot of lines to sift through manually and would waste a 
lot of time so I used the command ```/flag``` to search for the flag and got back the argument required as ```--aweh``` which I used to get the 
flag by using the command ```/challenge/challenge --aweh``` to get the required flag
```pwn.college{YnzkL_5ltykbI2-yssEfY3M-0Kq.dVTM4QDLxkDN1czW}```
## Challenge 5: Searching for manuals
In this challenge, I had to use the appropriate argument with the ```man``` command to know how to access the flag in ```/challenge/challenge```
### Method
 I first went through the ```man``` manual to find the appropriate argument which was
 ```-K, --global-apropos```
           ```Search for text in all manual pages.  This is a brute-force search,  and
              is likely to take some time; if you can, you should specify a section to
              reduce the number of pages that need to be searched.  Search  terms  may
              be  simple  strings (the default), or regular expressions if the --regex
              option is used.```
then I used the mentioned argument to read the ```challenge``` manual using the command ```man -K challenge``` which gave me information about
access to the flag which gave me the required argument as ```--mrpesb NUM``` with the ```NUM``` being ```941```
which I used in the command ```/challenge/challenge --mrpesb 941``` which gave me the required flag
```pwn.college{YmrpeKsTSQbYQcktCnJCl_e9RAh.dZTM4QDLxkDN1czW}```
## Challenge 6: Helpful Programs
In this challenge, I had to use the ```-h``` argument in the program ```/challenge/challenge```  to get the flag
### Method
I first ran the command ```/challenge/challenge -h``` which gave me information about all the arguments of the program
then I ran the command ```/challenge/challenge -p``` to get the value required to access the flag 
finally, I ran the command  ```/challenge/challenge -g 386``` to get the flag required
```pwn.college{UAfhh3qLbIgjQV_pjiAy_G8la6z.ddjM4QDLxkDN1czW}```
## Challenge 7: Help for Builtins 
In this challenge, I had to use builtins for a command to get the flag
### Method
I first ran the builtin ```help``` for the command ```challenge``` using the command ```help challenge```
which gave me the necessary arguments to get the flag which was the secret value ```MCD1fhLa``` for the argument ```--secret```
I ran the command ```challenge --secret MCD1fhLa``` to get the required flag which was 
```pwn.college{MCD1fhLaBYVijgwwclr-YtXmUMm.dRTM5QDLxkDN1czW}```
```
