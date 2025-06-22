# OverTheWire Wargames – Cybersecurity Practice Portfolio (LINUX PRACTICE) 

This repository documents my progress and what I have learnt through the [OverTheWire] (Bandit)  


- (LEVEL 1->2) - Is a command and it wont let you use "cat" unless it is using the full path (cat ./-)

- (LEVEL 3->4) To find human readable files use the command "file" to understand the type of file it is. ASCII text is human readable.

- (LEVEL 5->6) There is only 1 file with 1033b use command find with flag "-size" 1033c (c= bytes in this command)	

- (LEVEL 6->7) find / -type f -user bandit6 -group bandit7 -size 33c 2>/dev/null (find / searches all directory, -type f means only find files, and the others are filters)

- (LEVEL 7->8) cat data.txt | grep -w millionth (flag w makes sure it grabs the exact word millionth)	

- (LEVEL 8->9) cat data.txt | sort -d | uniq -u (-d flag sorts by duplicates but then the other pipe -u makes brings the unique one)

- (LEVEL 9->10)	cat data.txt | strings -w (-w flag helps find like certain text that is "human readable")

- (LEVEL 10->11)cat data.txt | base64 -d (base64 seems to be an encoding type which changes binary into more characters and -d flag uncodes it)		

- (LEVEL 11->12) cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m' (ROT13 is an algorithm that rotates 13 letters down the characters, tr means translate)

- (LEVEL 12->13) There is different types of compressing tools and file "file" helps you understand what it is; you have to decompress until find the password.

- (LEVEL 13->14) Connect through SSH as the user that has the permission using the key on the file and then read the file as the user with the permission.

- (LEVEL 14->15)  nc localhost 30000 (nc "netcat" opens a connection through a port so its listening,  source:localhost; port:30000)

- (LEVEL 15->16) openssl s_client -connect localhost:30001 (openssl for ssl (encryption communication) through localhost in port 30001)	


Still grinding. More levels coming soon...
