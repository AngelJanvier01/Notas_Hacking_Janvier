Puntos: 5pts
# Objetivo del Nivel

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/11/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/11/level1.flag.txt.enc) in the same directory too.`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/11/level1.py
--2024-03-03 05:40:08--  https://artifacts.picoctf.net/c/11/level1.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.128, 3.160.22.92, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 876 [application/octet-stream]
Saving to: 'level1.py'

level1.py                                                         100%[=============================================================================================================================================================>]     876  --.-KB/s    in 0s      

2024-03-03 05:40:08 (18.1 MB/s) - 'level1.py' saved [876/876]

janviier-picoctf@webshell:~$ wget 
wget: missing URL
Usage: wget [OPTION]... [URL]...

Try `wget --help' for more options.
janviier-picoctf@webshell:~$ 
janviier-picoctf@webshell:~$ wget 
wget: missing URL
Usage: wget [OPTION]... [URL]...

Try `wget --help' for more options.
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
--2024-03-03 05:40:31--  https://artifacts.picoctf.net/c/11/level1.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.43, 3.160.22.92, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 30 [application/octet-stream]
Saving to: 'level1.flag.txt.enc'

level1.flag.txt.enc                                               100%[=============================================================================================================================================================>]      30  --.-KB/s    in 0s      

2024-03-03 05:40:31 (16.9 MB/s) - 'level1.flag.txt.enc' saved [30/30]

janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  convertme.py  file  fixme1.py  fixme2.py  flag  level1.flag.txt.enc  level1.py  static  strings  warm
janviier-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: ^Z
[1]+  Stopped                 python level1.py
janviier-picoctf@webshell:~$ strings level1.flag.txt.enc 
janviier-picoctf@webshell:~$ file level1.flag.txt.enc 
level1.flag.txt.enc: data
janviier-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_fa343060}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/