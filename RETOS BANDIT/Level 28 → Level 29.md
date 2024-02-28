# Objetivo del Nivel

There is a git repository at `ssh://bandit28-git@localhost/home/bandit28-git/repo` via the port `2220`. The password for the user `bandit28-git` is the same as for the user `bandit28`.

Clone the repository and find the password for the next level.
# Datos de Acceso Al Nivel
bandit28 YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
# Solución

```bash

git clone ssh://bandit28git@localhost:2220/home/bandit28-git/repo
bandit28@bandit:/tmp/jaanviierGit$ cd repo
bandit28@bandit:/tmp/jaanviierGit/repo$ git log
commit 14f754b3ba6531a2b89df6ccae6446e8969a41f3 (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Thu Oct 5 06:19:41 2023 +0000

bandit28@bandit:/tmp/jaanviierGit/repo$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx
bandit28@bandit:/tmp/jaanviierGit/repo$ git checkout f08b9cc63fa1a4602fb065257633c2dae6e5651b
bandit28@bandit:/tmp/jaanviierGit/repo$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S

 ```

# Notas Adicionales
git
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