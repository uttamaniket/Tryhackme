find commond is the one of the best commond for finding directories and files

## Be more specific 

#1 Find all files whose name ends with ".xml"
Ans. find / -type f -name "*.xml"

#2 find all files in the /home directory (recursive) whose name is "user.txt" (case insensitive)
Ans. find /home -type f -iname user.txt


#3 Find all directories whose name contains the word "exploits"
Ans. find / -type d -name "*exploits*"

## Know exactly what you're looking for 

#1 Find all files owned by the user "kittycat"
Ans. find / -type f -user kittycat

#2 Find all files that are exactly 150 bytes in size
Ans.find / -type f -size 150c

#3 Find all files in the /home directory (recursive) with size less than 2 KiB’s and extension ".txt"
Ans. find /home -type f -size -2k -name "*.txt"

#4 Find all files that are exactly readable and writeable by the owner, and readable by everyone else (use octal format)
Ans. find / -type f -perm 644

#5 Find all files that are only readable by anyone (use octal format)
Ans. find / -type f -perm /444

#6 Find all files with write permission for the group "others", regardless of any other permissions, with extension ".sh" (use symbolic format)
Ans. find / -type f -perm -o=w -name "*.sh"

#7 Find all files in the /usr/bin directory (recursive) that are owned by root and have at least the SUID permission (use symbolic format)
Ans. find /usr/bin -type f -user root -perm -u=s

#8 Find all files that were not accessed in the last 10 days with extension ".png"
Ans.find / -type f -atime +10 -name "*.png"

#9 Find all files in the /usr/bin directory (recursive) that have been modified within the last 2 hours
Ans. find /usr/bin -type f -mmin -120
