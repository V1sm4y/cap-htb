# Writeup
So ofc we start off with an nmap scan. The one I like to use is :
```
nmap -sS -sV -sC <target_ip>
```
This does service scan , version scans and runs automated python scripts in that order
which gives you :
'''
21/tcp open  ftp     vsftpd 3.0.3
22/tcp open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.2 (Ubuntu Linux; protocol 2.0)
80/tcp open  http    gunicorn
'''
so three ports are open including a http server on port 80. Lets visit that.