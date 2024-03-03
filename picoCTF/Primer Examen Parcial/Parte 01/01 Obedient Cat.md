Puntos: 5pts
# Objetivo del Nivel

This file has a flag in plain sight (aka "in-the-clear"). [Download flag](https://mercury.picoctf.net/static/fb851c1858cc762bd4eed569013d7f00/flag).
# Pistas del Nivel
- Any hints about entering a command into the Terminal (such as the next one), will start with a '$'... everything after the dollar sign will be typed (or copy and pasted) into your Terminal.
- To get the file accessible in your shell, enter the following in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/fb851c1858cc762bd4eed569013d7f00/flag`
- $ man cat
# Solución/Resultado/Flag

```bash
==========================================================================

janviier-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/fb851c1858cc762bd4eed569013d7f00/flag
--2024-03-03 04:35:12--  https://mercury.picoctf.net/static/fb851c1858cc762bd4eed569013d7f00/flag
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag                                                              100%[=============================================================================================================================================================>]      34  --.-KB/s    in 0s      

2024-03-03 04:35:12 (17.9 MB/s) - 'flag' saved [34/34]

janviier-picoctf@webshell:~$ ls
README.txt  flag
janviier-picoctf@webshell:~$ cat flag
picoCTF{s4n1ty_v3r1f13d_28e8376d}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/147