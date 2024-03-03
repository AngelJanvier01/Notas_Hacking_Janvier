Puntos: 5pts
# Objetivo del Nivel

Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) without running it?
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings
--2024-03-03 05:29:39--  https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 776032 (758K) [application/octet-stream]
Saving to: 'strings'

strings                                                           100%[=============================================================================================================================================================>] 757.84K  1.86MB/s    in 0.4s    

2024-03-03 05:29:39 (1.86 MB/s) - 'strings' saved [776032/776032]

janviier-picoctf@webshell:~$ ls
Addadshashanammu  Addadshashanammu.zip  README.txt  code.py  codebook.txt  convertme.py  file  fixme1.py  flag  static  strings  warm
janviier-picoctf@webshell:~$ cd strings
-bash: cd: strings: Not a directory
janviier-picoctf@webshell:~$ strings strings | grep pico
picoCTF{5tRIng5_1T_d66c7bb7}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/