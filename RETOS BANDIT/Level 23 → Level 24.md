# Objetivo del Nivel

A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
# Datos de Acceso Al Nivel
bandit23 QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G
# Solución

```bash
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ nano bandit24_pass.sh
Unable to create directory /home/bandit23/.local/share/nano/: No such file or directory
It is required for saving/loading search history or cursor positions.

bandit23@bandit:/tmp/tmp.Bd906nDXgT$ nano bandit24_pass.sh
Unable to create directory /home/bandit23/.local/share/nano/: No such file or directory
It is required for saving/loading search history or cursor positions.

bandit23@bandit:/tmp/tmp.Bd906nDXgT$ ls
bandit24_pass.sh
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ hmod +rx bandit24_pass.sh 
Command 'hmod' not found, did you mean:
  command 'kmod' from deb kmod (29-1ubuntu1)
  command 'qmod' from deb gridengine-client (8.1.9+dfsg-10build1)
  command 'chmod' from deb coreutils (8.32-4.1ubuntu1)
  command 'jmod' from deb openjdk-11-jdk-headless (11.0.20.1+1-0ubuntu1~22.04)
  command 'jmod' from deb openjdk-17-jdk-headless (17.0.8.1+1~us1-0ubuntu1~22.04)
  command 'jmod' from deb openjdk-18-jdk-headless (18.0.2+9-2~22.04)
  command 'jmod' from deb openjdk-19-jdk-headless (19.0.2+7-0ubuntu3~22.04)
  command 'mod' from deb monodoc-base (6.8.0.105+dfsg-3.2)
Try: apt install <deb name>
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod +rx bandit24_pass.sh 
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod 777 /tmp/tmp.Bd906nDXgT
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ touch password
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod +rwx password 
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ ls -la
total 408
drwxrwxrwx   2 bandit23 bandit23   4096 Feb 27 04:36 .
drwxrwx-wt 638 root     root     405504 Feb 27 04:36 ..
-rwxrwxr-x   1 bandit23 bandit23     74 Feb 27 04:35 bandit24_pass.sh
-rwxrwxr-x   1 bandit23 bandit23      0 Feb 27 04:36 password
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ cp bandit24_pass.sh /var/spool/bandit24/bandit24_pass.sh
cp: cannot create regular file '/var/spool/bandit24/bandit24_pass.sh': Operation not permitted
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ cp bandit24_pass.sh /var/spool/bandit24/bandit24_pass.sh
cp: cannot create regular file '/var/spool/bandit24/bandit24_pass.sh': Operation not permitted
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod +rx bandit24_pass.sh 
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod 777 /tmp/tmp.Bd906nDXgT
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ ls
bandit24_pass.sh  password
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ hmod +rwx password 
Command 'hmod' not found, did you mean:
  command 'kmod' from deb kmod (29-1ubuntu1)
  command 'chmod' from deb coreutils (8.32-4.1ubuntu1)
  command 'jmod' from deb openjdk-11-jdk-headless (11.0.20.1+1-0ubuntu1~22.04)
  command 'jmod' from deb openjdk-17-jdk-headless (17.0.8.1+1~us1-0ubuntu1~22.04)
  command 'jmod' from deb openjdk-18-jdk-headless (18.0.2+9-2~22.04)
  command 'jmod' from deb openjdk-19-jdk-headless (19.0.2+7-0ubuntu3~22.04)
  command 'qmod' from deb gridengine-client (8.1.9+dfsg-10build1)
  command 'mod' from deb monodoc-base (6.8.0.105+dfsg-3.2)
Try: apt install <deb name>
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ chmod +rwx password 
bandit23@bandit:/tmp/tmp.Bd906nDXgT$ cp bandit24_pass.sh /var/spool/bandit24/bandit24_pass.sh
VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
```

# Notas Adicionales
cron, crontab, crontab(5) (use “man 5 crontab” to access this)
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