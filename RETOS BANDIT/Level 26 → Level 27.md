# Objetivo del Nivel

Good job getting a shell! Now hurry and grab the password for bandit27!
# Datos de Acceso Al Nivel
bandit26 c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1
# Solución

```bash

:set shell=/bin/bash 
	:shell

bandit26@bandit:~$ ls
bandit27-do  text.txt
bandit26@bandit:~$  echo 'cat /etc/bandit_pass/bandit27' > /tmp/getpass27.sh
bandit26@bandit:~$ chmod a+x /tmp/getpass27.sh
bandit26@bandit:~$ ./bandit27-do /tmp/getpass27.sh
cat: /etc/bandit_pass/bandit27: Permission denied
bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27
YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
bandit26@bandit:~$ 

 ```

# Notas Adicionales
ls
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