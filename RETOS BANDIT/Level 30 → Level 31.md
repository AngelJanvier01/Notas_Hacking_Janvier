# Objetivo del Nivel

There is a git repository at `ssh://bandit30-git@localhost/home/bandit30-git/repo` via the port `2220`. The password for the user `bandit30-git` is the same as for the user `bandit30`.

Clone the repository and find the password for the next level.
# Datos de Acceso Al Nivel
bandit30 xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS
# Solución

```bash

bandit30@bandit:~$ mkdir /tmp/jaanviier-gitt
bandit30@bandit:~$ cd /tmp/jaanviier-gitt
bandit30@bandit:/tmp/jaanviier-gitt$ git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit30/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit30/.ssh/known_hosts).
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

bandit30-git@localhost's password:
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), done.
bandit30@bandit:/tmp/jaanviier-gitt$ cd repo
bandit30@bandit:/tmp/jaanviier-gitt/repo$ ls -la
total 16
drwxrwxr-x 3 bandit30 bandit30 4096 Feb 24 22:29 .
drwxrwxr-x 3 bandit30 bandit30 4096 Feb 24 22:29 ..
drwxrwxr-x 8 bandit30 bandit30 4096 Feb 24 22:29 .git
-rw-rw-r-- 1 bandit30 bandit30   30 Feb 24 22:29 README.md
bandit30@bandit:/tmp/jaanviier-gitt/repo$ cat README.md
just an epmty file... muahaha
bandit30@bandit:/tmp/jaanviier-gitt/repo$ git branch
* master
bandit30@bandit:/tmp/jaanviier-gitt/repo$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/master
bandit30@bandit:/tmp/jaanviier-gitt/repo$ git log
commit d39631d73f786269b895ae9a7b14760cbf40a99f (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Thu Oct 5 06:19:45 2023 +0000

    initial commit of README.md
bandit30@bandit:/tmp/jaanviier-gitt/repo$ git tag
secret
bandit30@bandit:/tmp/jaanviier-gitt/repo$ git show secret
OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt

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