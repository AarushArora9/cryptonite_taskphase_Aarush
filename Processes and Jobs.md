# Hello
## Challenge 1: Listing Processes
In this challenge I had to use the ```ps``` command with appropriate arguments to get the hidden file and call it to get the flag
### Method
I did so using the arguments ```-ef``` which list all the running processes in which the process running within the ```/challenge``` directory was named ```/challenge/14712-run-31605``` which I called using the
same command which gave me the flag ```pwn.college{wfdZxBol__zFFvfM5pHj0pi8Do1.dhzM4QDLxkDN1czW}```
## Challenge 2: Killing processes
In this challenge I had to kill a specific process to run a particular process that would give me the required flag
### Method
I ran the ```ps -ef``` command first to list all the running processes and nothing the PID of process ```/challenge/dont_run``` as 74 which I terminated using the command ```kill 74```
then I executed ```/challenge/run``` to get the required flag which was ```pwn.college{4ezPTPDppQgoJzw1RD49rZ7bYqY.dJDN4QDLxkDN1czW}```
## Challenge 3: Interrupting processes
In this challenge I had to interrupt a running command to get the flag
### Method
I first ran the command ```/challenge/run``` and then I had to interrupt it using Ctrl+C which gave me the required flag ```pwn.college{sMq-B-sR3hWDxl7waJAewmz887g.dNDN4QDLxkDN1czW}```
## Challenge 4: Suspending processes 
In this challenge I had to suspend a running process to get the flag
### Method
I first ran the command ```/challenge/run``` and then I suspended it using Ctrl+Z and then I ran it again to get the flag ```pwn.college{4Aa4uJzpjWlDocxDnBR6_oEBuvi.dVDN4QDLxkDN1czW}```
## Challenge 5: Resuming Processes
In this challenge I had to resume a suspended process to get the flag
### Method
I first ran the command ```/challenge/run``` and then suspended it using Ctrl+Z and then resumed it using the command ```fg``` to get the required flag
```pwn.college{gRyoJmYMiQ4AfctwekwMA_AcS6H.dZDN4QDLxkDN1czW}```
## Challenge 6: Backgrounding processes
In this challenge I had to run a command, suspend it, push it to the background, and then finally rerun it to get the flag
### Method
I first ran the command ```/challenge/run``` and then suspended it using Ctrl+Z and then pushed it to the background using the command ```bg``` then I reran it to get the required flag
```pwn.college{46yCoIiz7U4RTmHuWcUE8_XNuPn.ddDN4QDLxkDN1czW}```
## Challenge 7: Foregrounding Processes
In this challenge I had to foreground a backgrounded process which I previously also suspended
### Method
I first ran the command ```/challenge/run``` and then suspended it using Ctrl+Z and then pushed it to the background using the command ```bg``` and then I foregrounded it using the command ```fg``` and got 
the required flag which was ```pwn.college{02JZ1y8nDJzZ9uOb3R4APTYQo4-.dhDN4QDLxkDN1czW}```
## Challenge 8: Starting Backgrounded Processes
In this challenge I had to directly start a process in the background to get the flag
### Method
To do so I had to run the command ```/challenge/run``` with argument ```&``` ran the command ```/challenge/run &``` which directly gave me the flag which was
```pwn.college{0HnfnxFhp1BJrlVYZYV3VLspIiQ.dlDN4QDLxkDN1czW}```
## Challenge 9: Process exit codes
In this challenge I had to run a command, get its exit code, and pass the exit code as an argument to another command to get the flag
### Method
To do so I first ran the command ```/challenge/get-code``` which exited with an error code, I read the error code using the command ```ech $?``` which gave me value ```205``` which I passed as an argument
to the command ```/challenge/submit-code``` as follows ```/challenge/submit-code 205``` to get the flag 
```pwn.college{8awIZ7k84IPbwMJ1EqbgjTkQdxt.dljN4UDLxkDN1czW}```
