# Hello
## Challenge 1: Becoming root with su
In this challenge I had to change the user access using the ```su``` command and get the flag
### Method 
I used the ```su``` command and filled in the required authentication password ```hack-the-planet``` to change the user access then I printed the file containing the flag 
using the command ```cat /flag``` to get the flag:
```pwn.college{0YGD8SZPJnFLkcOv5I_wIYtXfkv.dVTN0UDLxkDN1czW}```
## Challenge 2: Other users with su
In this challenge I had to switch to another user using ```su``` and run a command to get the flag
### Method
To do so I used the ```su zardus``` command to change my user to zardus and filled in the required authentication ```dont-hack-me``` to change the user access and ran the command 
```/challenge/run``` to get the flag
```pwn.college{0s9_G6QF-PIscjFvwtOYMR62sQM.dZTN0UDLxkDN1czW}```
## Challenge 3: Cracking passwords
In this challenge I had to change my user to ```zardus``` by getting the required password using the ```john``` command
### Method
To do so I first ran the command ```john /challenge/shadow-leak``` because that's where passwords are stored, doing so gave me the required password as ```aardvark``` which I used to ```su``` 
and change me user to ```zardus```, then I ran the ```/challenge/run``` command to get the flag
```pwn.college{Esy4HfdtlgIQRg_rcHC0i7i4bBz.ddTN0UDLxkDN1czW}```
## Challenge 4: Using Sudo
In this challenge I had to use the ```sudo``` command to get the flag
### Method 
I did so by reading the ```/flag``` file through ```sudo``` using the command ```sudo cat /flag``` which gave me the flag
```pwn.college{EO_os7t4QpSoD3PjX6-ySg4TNhP.dhTN0UDLxkDN1czW}```
