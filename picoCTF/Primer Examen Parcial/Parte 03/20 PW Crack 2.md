Puntos: 5pts
# Objetivo del Nivel

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/13/level2.py
--2024-03-03 05:43:47--  https://artifacts.picoctf.net/c/13/level2.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.43, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 914 [application/octet-stream]
Saving to: 'level2.py'

level2.py                                                         100%[=============================================================================================================================================================>]     914  --.-KB/s    in 0s      

2024-03-03 05:43:47 (240 MB/s) - 'level2.py' saved [914/914]

janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/13/level2.flag.txt.enc
--2024-03-03 05:43:59--  https://artifacts.picoctf.net/c/13/level2.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.43, 3.160.22.92, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 31 [application/octet-stream]
Saving to: 'level2.flag.txt.enc'

level2.flag.txt.enc                                               100%[=============================================================================================================================================================>]      31  --.-KB/s    in 0s      

2024-03-03 05:43:59 (13.5 MB/s) - 'level2.flag.txt.enc' saved [31/31]

janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  convertme.py  file  fixme1.py  fixme2.py  flag  level1.flag.txt.enc  level1.py  level2.flag.txt.enc  level2.py  static  strings  warm
janviier-picoctf@webshell:~$ nano level2.py 
janviier-picoctf@webshell:~$ python level2.py 
Please enter correct password for flag: de76
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/