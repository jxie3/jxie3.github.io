# Getting into CTFs: Day 1 #

I finally started learning some of the knowledge needed for CTFs, after hearing about how it's a fun, puzzle-y, and also great for learning programming (which I desperately need to get better at before I start college). Today, I just looked at the first few chapters of the [CTF Primer] (https://primer.picoctf.org/#_introduction) on picoCTF and learned some essential skills.

## Man ##

`man` (short for Manual, I think) is the command for looking up commands! For example, in order to look up the `grep` command, simply do `man grep` and a whole page of useful info will pop up, including what `grep` does and how to format `grep` commands.

## Grep and Find ##

Grep and Find are super useful for searching files and directories. 

`grep` can be used to find occurences of strings in a text file. For example, `grep 'picoCTF' file.txt` will return all the lines that have the string 'picoCTF' in them. For example, `grep 'string' filename.txt` will print all the lines that contain 'string' in the file filename.txt. Note that the string you want to search for must be in quotes! I didn't do this at first and was confused about why it wasn't working.

`find` can be used to go through files starting from the directory you are in. For example, `find ~ -name "*.txt"` starts in the home directory and finds all files that end with `.txt` (the * there is a regular expression). Note that you should include the "-name", otherwise the command will think that the file you're searching for is the directory you want to start from. 
