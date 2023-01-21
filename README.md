# CVE-2023-22809

## sudo Privilege escalation

Affected sudo versions: 1.8.0 to 1.9.12p1 

This script automates the exploitation of the CVE-2023-22809 vulnerability to 
gain a root shell. 

The script checks if the current user has access to run the `sudoedit` or 
`sudo -e` command for some file with root privileges. If it does it opens the 
sudoers file for the attacker to introduce the privilege escalation policy 
for the current user and get a root shell.
