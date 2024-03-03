Puntos: 5pts
# Objetivo del Nivel

Run the Python script and convert the given number from decimal to binary to get the flag.[Download Python script](https://artifacts.picoctf.net/c/24/convertme.py)
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  flag  static  warm
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/24/convertme.py
--2024-03-03 05:20:19--  https://artifacts.picoctf.net/c/24/convertme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.128, 3.160.22.16, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1189 (1.2K) [application/octet-stream]
Saving to: 'convertme.py'

convertme.py                                                      100%[=============================================================================================================================================================>]   1.16K  --.-KB/s    in 0s      

2024-03-03 05:20:20 (524 MB/s) - 'convertme.py' saved [1189/1189]

janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  convertme.py  flag  static  warm
janviier-picoctf@webshell:~$ python convertme.py 
If 52 is in decimal base, what is it in binary base?
Answer: 111011
59 and 52 are not equal.
janviier-picoctf@webshell:~$ python convertme.py 
If 78 is in decimal base, what is it in binary base?
Answer: ^CTraceback (most recent call last):
  File "/home/janviier-picoctf/convertme.py", line 23, in <module>
    ans = input('Answer: ')
KeyboardInterrupt

janviier-picoctf@webshell:~$ python convertme.py 
If 14 is in decimal base, what is it in binary base?
Answer: 1110 
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_722f6b39}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/