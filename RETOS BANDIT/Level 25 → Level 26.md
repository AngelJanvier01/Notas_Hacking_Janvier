# Objetivo del Nivel

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not **/bin/bash**, but something else. Find out what it is, how it works and how to break out of it.
# Datos de Acceso Al Nivel
bandit25 p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d
# Solución

```bash

bandit25@bandit:~$ cat /etc/passwd | grep bandit26  
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext  
bandit25@bandit:~$

bandit25@bandit:~$ cat /usr/bin/showtext  
#!/bin/shexport TERM=linuxmore ~/text.txt  
exit 0  

```

# Notas Adicionales
ssh, cat, more, vi, ls, id, pwd
# Referencias
- [Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
- [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](http://tldp.org/LDP/abs/html/special-chars.html)
- [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)
- [Base64 on Wikipedia](https://en.wikipedia.org/wiki/Base64)
- [Rot13 on Wikipedia](https://en.wikipedia.org/wiki/Rot13)
- [Hex dump on Wikipedia](https://en.wikipedia.org/wiki/Hex_dump)
- [SSH/OpenSSH/Keys](https://help.ubuntu.com/community/SSH/OpenSSH/Keys)
- [How the Internet works in 5 minutes (YouTube)](https://www.youtube.com/watch?v=7_LPdttKXPc) (Not completely accurate, but good enough for beginners)
- [IP Addresses](http://computer.howstuffworks.com/web-server5.htm)
- [IP Address on Wikipedia](https://en.wikipedia.org/wiki/IP_address)
- [Localhost on Wikipedia](https://en.wikipedia.org/wiki/Localhost)
- [Ports](http://computer.howstuffworks.com/web-server8.htm)
- [Port (computer networking) on Wikipedia](https://en.wikipedia.org/wiki/Port_(computer_networking))
- [Secure Socket Layer/Transport Layer Security on Wikipedia](https://en.wikipedia.org/wiki/Secure_Socket_Layer)
- [OpenSSL Cookbook - Testing with OpenSSL](https://www.feistyduck.com/library/openssl-cookbook/online/ch-testing-with-openssl.html)
- [Port scanner on Wikipedia](https://en.wikipedia.org/wiki/Port_scanner)
- [setuid on Wikipedia](https://en.wikipedia.org/wiki/Setuid)
- 