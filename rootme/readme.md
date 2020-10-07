 IP address 10.10.255.168

nmap scan result open port 80 http and 22 ssh

# Got /panel/ dir inside our server using gobuster

After uploading reverse shell

1. got Access to linux machine (User Access)

For checking -perm root user :
We Got /usr/bin/python for prvese 

python -c 'import pty; pty.spawn("/bin/bash")'
bash-4.4$ /usr/bin/python -c 'import os; os.execl("/bin/sh", "sh", "-p")'

these two cmd help to get shell & get suid for previlege Escalation.




#1.1 Scan the machine, how many ports are open?
Ans. 2

#1.2 What version of Apache are running?
Ans. 2.4.49

#1.3 What service is running on port 22?
Ans. 22

#1.4 What is the hidden directory?
Ans. /panel/

#2.1 user.txt 
Ans. THM{y0u_g0t_a_sh3ll}

#3.1 Search for files with SUID permission, which file is weird? 
Ans. /usr/bin/python

#3.2 root.txt
Ans. THM{pr1v1l3g3_3sc4l4t10n}
