# Reversing-ELF
tryhackme room to practice reverse engineering to find hidden stuff
#Reversing ELF


1-1st challenge

it was simple the file was executable
using chmod +x file i got the flag
flag{not_that_kind_of_elf}

2-2nd challenge

this file is executible : using file crackme2
when i run the crackme2 then it shows usage : ./crackme password 
means i need password to run this file
using vim and strigs i got password 
super_secret_password

and flag after executing command 

flag{if_i_submit_this_flag_then_i_will_get_points}

3-3rd challenge


this file is also executible

we again need password !!! to run this file lets try some basic reverse 
engineering 

found a base64 encoded string in vim or(using strings <file> command)
base64 string:ZjByX3kwdXJfNWVjMG5kX2xlNTVvbl91bmJhc2U2NF80bGxfN2gzXzdoMW5nNQ==


after encrypting it got a flag
f0r_y0ur_5ec0nd_le55on_unbase64_4ll_7h3_7h1ng5



4-4th challenge
again the file is executible and again need password for execution
this time vim or strings command doesnot giving any password

but the hint is:This time the string is hidden and we used strcmp


now using gdb debugger to debug the binary
IDA / Radare2 :this is similar to ghidra but it runs inside of linux

