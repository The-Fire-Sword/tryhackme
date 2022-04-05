
# ROOTME

### Scan the machine, how many ports are open?
```bash
nmap "IP"
 ```

### What version of Apache is running?
```bash
  nmap f -sSVC "IP" 

- "-sV" (version detect)
 ```

### Find a form to upload and get a reverse shell, and find the flag.
```bash
- File reverse shell .php (rename file)
 ```
## Encontrar arquivos com permissoes 
#### Search for files with SUID permission, which file is weird?
```bash
find / -perm -u=s -ls 2>/dev/null
```
### Melhorar a Shell
```bash
python3 -c 'import pty; pty.spawn("/bin/bash")'
ctrl + z
stty raw -echo && fg
export TERM=xterm
```

## Gobuster 
###  What is the hidden directory?
```bash
sudo gobuster dir -u http://0.0.0.0/ -x txt,php,html -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -t 200 2> /dev/null
 ```   
## Find File
#### root.txt
```bash
find / -type f -name root.txt
 ``` 
## Site SUID
#### Find a form to escalate your privileges.
```bash
https://gtfobins.github.io/gtfobins/python/
 ```  