# Linux Commands

| Command | Description |
| --- | --- |
| sudo apt-get update && sudo apt-get upgrade && sudo apt-get autoremove | update apt package list, upgrade installed packages and autoremove unused packages |
| sudo apt-get --with-new-pkgs upgrade | upgrade “held back” packages. These are packages that have new dependancies that need to be installed for the package to be upgraded. |

## Troubleshooting port conflicts

| Command | Description |
| --- | --- |
| netstat -vanp tcp \| grep 5000 | checks for whats listening on TCP 5000 port |
| lsof -i tcp:5000 | checks for whats listening on TCP port 5000 on macOS |
| sudo netstat -tulpn \| grep 5000 | |

## User Management

| Command | Description |
| --- | --- |
| adduser -m <username> | make new user account with home directory |
| passwd <username> | set password for user account |
| userdel -r <username> | delete user account |
| usermod -a -G sudo <username> | add user account to "sudo" user group |

## Firewall Management

| Command | Description |
| --- | --- |
| sudo ufw app list | |
| sudo ufw allow 3306 | |
| sudo ufw delete allow 443 | |
| sudo ufw disable | |

## SSH

| Command | Description |
| --- | --- |
| ssh-keygen -t rsa -b 4096 -C "<e-mail address>" | generate SSH key using specified email |

## Backup/File Transfer Using RSync

| Command | Description |
| --- | --- |
| sudo rsync -avzx -e 'ssh -p 2222' --progress <source path> <user@hostname>:/<volume name>/<folder name> | transfer files from source path to destination host using specified SSH port, TCP 2222 |
