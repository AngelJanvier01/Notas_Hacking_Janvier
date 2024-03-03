Puntos: 5pts
# Objetivo del Nivel

Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/17/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) in the same directory too.There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/17/level3.py
--2024-03-03 05:45:51--  https://artifacts.picoctf.net/c/17/level3.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.128, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1337 (1.3K) [application/octet-stream]
Saving to: 'level3.py'

level3.py                                                         100%[=============================================================================================================================================================>]   1.31K  --.-KB/s    in 0s      

2024-03-03 05:45:51 (65.4 MB/s) - 'level3.py' saved [1337/1337]

janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/17/level3.flag.txt.enc
--2024-03-03 05:45:59--  https://artifacts.picoctf.net/c/17/level3.flag.txt.enc
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.43, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 31 [application/octet-stream]
Saving to: 'level3.flag.txt.enc'

level3.flag.txt.enc                                               100%[=============================================================================================================================================================>]      31  --.-KB/s    in 0s      

2024-03-03 05:45:59 (13.0 MB/s) - 'level3.flag.txt.enc' saved [31/31]

janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/17/level3.hash.bin
--2024-03-03 05:46:06--  https://artifacts.picoctf.net/c/17/level3.hash.bin
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.128, 3.160.22.43, 3.160.22.16, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.128|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 16 [application/octet-stream]
Saving to: 'level3.hash.bin'

level3.hash.bin                                                   100%[=============================================================================================================================================================>]      16  --.-KB/s    in 0s      

2024-03-03 05:46:06 (217 KB/s) - 'level3.hash.bin' saved [16/16]

janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  convertme.py  file  fixme1.py  fixme2.py  flag  level1.flag.txt.enc  level1.py  level2.flag.txt.enc  level2.py  level3.flag.txt.enc  level3.hash.bin  level3.py  static  strings  warm
janviier-picoctf@webshell:~$ nano lev
janviier-picoctf@webshell:~$ nano level3.py 
janviier-picoctf@webshell:~$ python level3.py 
Please enter correct password for flag: 87ab
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_cd6ed2eb}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/