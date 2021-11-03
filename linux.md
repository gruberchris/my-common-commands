# Linux Commands

## Troubleshooting port conflicts

| Command | Description |
| --- | --- |
| netstat -vanp tcp \| grep 5000 | checks for whats listening on TCP 5000 port |
| lsof -i tcp:5000 | checks for whats listening on TCP port 5000 on macOS |
| sudo netstat -tulpn \| grep 5000 | |