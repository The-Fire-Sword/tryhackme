
# ROOTME

Tryhackme room ROOTME

### Encontrar arquivos com permissoes 

```bash
find / -perm -u=s -ls 2>/dev/null
```
### Entrar no servidor

```bash
python3 -c 'import pty; pty.spawn("/bin/bash")'
ctrl + z
stty raw -echo && fg
export TERM=xterm
```

### Wordilist de diretorios (buscador de diretorios) 

```bash
sudo gobuster dir -u http://0.0.0.0/ -x txt,php,html -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -t 200 2> /dev/null
 ```   

### Site SUID

```bash
https://gtfobins.github.io/gtfobins/python/
 ```  