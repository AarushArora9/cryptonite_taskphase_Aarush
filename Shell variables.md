# Hello
## Challenge 1: Printing Variables
In this challenge, I had to print a flag stored in a variable to complete the challenge
### Method
I used the command ```echo``` to print the variable by prepending the variable name with the operator ```$``` which gave me the command as ```echo $FLAG``` and provided the required flag which was
```pwn.college{M3fSgky33FDvIff5XUdLakCWSDT.ddTN1QDLxkDN1czW}```
## Challenge 2: Setting variables
In this challenge, I had to set the variable with a certain specified value to get the flag
### Method
I can directly name a variable in the command line and specify the given value so I just used the command ```PWN=COLLEGE``` to get the reuired flag which was
```pwn.college{UcRQDnTLu2DGCzTOife_RmG65sN.dlTN1QDLxkDN1czW}```
## Challenge 3: Multi-word variables
In this challenge, I had to assign the variable with a specified multi-word value to get the required flag
### Method
In this challenge, I had to use quotes to assign the value to the variable since the method in the previous challenge only works for single word so I had to use the command ```PWN="COLLEGE YEAH"```
to get the required flag which was ```pwn.college{0wNp3x_ibDf-YIZDzIAMV-VPpGQ.dBjN1QDLxkDN1czW}```
## Challenge 4: Exporting variables
In this challenge I had to export a variable with a specified value and use another variable to store another specified value
### Method
since I had to export one of the variables I did that in a single line command ```export PWN=COLLEGE``` and set the value of the other variable using the command ```COLLEGE=PWN``` and ran the 
required command ```/challenge/run``` to get the flag ```pwn.college{kfpqwFFu0qOETDDBip3t4nfBfGT.dJjN1QDLxkDN1czW}```
## Challenge 5: Printing exported variables
In this challenge I had to print an exported variable using ```env``` command
### Method
I used the variable name with ```$``` operator to access the content of the flag while using the command so the overall command was ```env $FLAG``` which gave me the flag
```pwn.college{Esir7UgtAler4j_LMNMacA9g38m.dhTN1QDLxkDN1czW}```
## Challenge 6: Storing Command Output
In this challenge I had to store the output of a command in a variable and then print the variable to get the flag
### Method
I used the the ```$``` to access the content of the ```/challenge/run``` command and store it in the variable ```PWN``` using the command ```PWN=$(/challenge/run)``` and print the contents
of the variable using ```echo "$FLAG"``` to get the flag ```pwn.college{4cO68MVbr9GC2xiviB-UbLw7dqd.dVzN0UDLxkDN1czW}```
## Challenge 7: Reading Input
In this challenge I had to set a specified value to a variable using the ```read``` command
### Method
I did so using the command ```read PWN``` which let me read a value into the variable which I set to ```COLLEGE``` as specified which provided me with the required flag
```pwn.college{odn6qNHx6HZT5nUS73S3h64UPGa.dhzN1QDLxkDN1czW}```
## Challenge 8: Reading Files
In this challenge I had to read a file into a variable to get the flag
### Method
I did so using the ```<``` to read the file into variable ```PWN``` which I did so using the command ```read PWN </challenge/read_me``` which gave me the flag
```pwn.college{ws5p-CdcjqNXok9xtlsHCnQhf-Z.dBjM4QDLxkDN1czW}```

