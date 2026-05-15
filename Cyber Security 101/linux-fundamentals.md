# Linux Fundamentals

------------------

Linux is based on ***UNIX*** operating systems. It was created in 1991, and it is open sourced.
It comes equiped with GUI, but it's main usage is in the Terminal, or CLI (command-line interface)

### Some of the most basic **linux** commands are:
```linux
echo - 	output any text that we provide
whoami - find out what user we're currently logged in as!
ls - listing
cd - change directory
cat - concatenate
pwd - print working directory
find - find files based on set parameters
grep - search for specific text patterns within files or command output
```

As there are many commands we use, there are also many **shell operators**:
```linux
& -  run commands in the background of your terminal
&& - combine multiple commands together in one line of your terminal
> - redirector - take the output from a command (such as using cat to output a file) and direct it elsewhere
>> - appends the output rather than replacing (meaning nothing is overwritten)
```

## SSH - Secure Shell 

For the first time in my life, after hearing about it countless times, I used SSH protocol. It's purpose is to remotely "connect" and execute commands on another device.
Syntax for using this protocol is **`ssh user@user-ip`**. After executing that command we are asked to trust the host and provide the account password. After all that, we are _connected_.

## Flags and Switches

All Linux commands accept additional insturction sets which are called flags or switches. Some of them are used all the time while others have a special usecase. Best way to learn about them is through the _manual_ page of the given command.

Example
```linux
man ls - opens a manual page for the ls command
```
