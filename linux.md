# Linux Commands

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
