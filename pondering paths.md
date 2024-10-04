# Hello
In this module, I learnt the basics of Linux file paths
## Challenge 1: The Root
In this challenge, I had to use ```/``` to access the file system and the command I had to access the ```pwn``` file.
### Method
The way I did this using the terminal is that I used the following command
```
/pwn
```
to get the following flag which I used to complete the challenge
```
pwn.college{kllrqU73p5v_CO6n47EgDNztjwC.dhzN5QDLxkDN1czW}
```
## Challenge 2: Program and Absolute Paths
In this challenge, I had to access the sub-directory ```run``` in the directory ```challenge``` which was situated in the root directory
### Method
I did so by invoking its absolute path in the root directory
```/challenge/run```
and getting the flag
```pwn.college{w3dNdS7PYAEqFd-hQA8k55KmqRz.dVDN1QDLxkDN1czW}```
by which I completed the challenge
## Challenge 3: Position thy self
In this challenge I had to use the  change directory ```cd``` command to navigate around directories, also I learned the use of ```~``` 
which is used to show the current position where the shell is located at
### Method
I used the ```/challenge/run``` command using the absolute path of ```challenge``` first which told me that I needed to change my directory to ```tmp```
which I did so using the command ```cd /tmp``` using the absolute path of tmp which is ```/tmp```
then I again executed the command I used earlier again using the absolute path of run directory
``` /challenge/run```
which gave me the following flag required for the problem
```pwn.college{oRk2_FdLbmDhNdl-39GwSGpUMmq.dZDN1QDLxkDN1czW}```
## Challenge 4: Position elsewhere
In this challenge, I was required to tinker further with the change directory ```cd``` command and absolute paths of files
### Method
I used the ```/challenge/run``` command using the absolute path of ```challenge``` first which told me that I needed to change my directory to ```/usr/bin```
which I did so using the command ```cd /usr/bin``` using the absolute path of tmp which is ```/tmp```
then I again executed the command I used earlier again using the absolute path of run directory
``` /challenge/run```
which gave me the following flag required for the problem
``` pwn.college{k3ILFgJKdq3Da-qR4BEmPckD6_O.ddDN1QDLxkDN1czW}```
## Challenger 5: Position yet elsewhere
In this challenge, I had to yet again play around with the change directory ```cd``` command and absolute paths to get the flag
### Method
I used the ```/challenge/run``` command using the absolute path of ```challenge``` first which told me that I needed to change my directory to ```tmp```
which I did so using the command ```cd /tmp``` using the absolute path of tmp which is ```/tmp```
then I again executed the command I used earlier again using the absolute path of run directory
``` /challenge/run```
which gave me the following flag required for the problem
```pwn.college{4t1s33j3e-GF3st0aBfN0xekJ0q.dhDN1QDLxkDN1czW}```
## Challenge 6: implicit relative paths, from /
In this challenge, I had to apply the concept of implicit relative paths by changing my Current Working Directory (CWD)
### Method
First I changed my current directory to my current working directory using the following command
```cd /```
and then I invoked the file using its implicit relative path in the CWD
```challenge challenge/run```
which gave me the following flag required to complete the challenge
```pwn.college{4UERzBYQZa8rtbTyQ9FdcvJKQS4.dlDN1QDLxkDN1czW}```
## Challenge 7: explicit relative paths, from ./
In this challenge, I had to use  the concept of explicit relative paths and apply them from ```/```
### Method
First I changed my directory to ```/``` using the command 
```cd /```
then I used the explicit relative path to invoke the file 
```./challenge/run```
which gave me the following flag required to complete the challenge
```pwn.college{0EfVUwA4Pm1oHcrD1DolLD10Unf.dBTN1QDLxkDN1czW}```
## Challenge 8: implicit relative path
In this challenge, I had to use the implicit relative path concept and run the command from the ```challenge``` directory.
### Method 
I first changed my directory to ```challenge```
using command ```cd /challenge```
then I tried to execute the command ```run``` as is which gave me an error
```bash: run: command not found ```
because Linux doesn't allow naked paths 
there I had to use ```./``` to convert it to an implicit relative path which was executed to yield the following flag
```pwn.college{UGJ9UQoZs0p_9bI8WNHiRsXZ6B7.dFTN1QDLxkDN1czW}```
## Challenge 9: home sweet home
In this challenge, I had to write a file containing the flag by executing the program at ```/challenge/run```.
This program made use of absolute paths in the context of the home directory and argument constraints provided
### Method
I first changed my directory to ```challenge```
using the command ```cd /challenge```
and since naked paths are not allowed in Linux I used the implicit relative path and created a file using the command
```./run ~/a```
which give me the following flag required to complete the challenge
```pwn.college{QiA5rZF5tkECRK_MTlEJYsU3_UQ.dNzM4QDLxkDN1czW}```



