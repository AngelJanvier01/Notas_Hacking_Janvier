Puntos: 50pts
# Objetivo del Nivel

This [garden](https://jupiter.challenges.picoctf.org/static/d0e1ffb10fc0017c6a82c57900f3ffe3/garden.jpg) contains more than it seems.

# Pistas del Nivel

- You should have enough hints to find the files, don't run a brute forcer.
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/d0e1ffb10fc0017c6a82c57900f3ffe3/garden.jpg
--2024-03-15 01:08:28--  https://jupiter.challenges.picoctf.org/static/d0e1ffb10fc0017c6a82c57900f3ffe3/garden.jpg
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 2295192 (2.2M) [application/octet-stream]
Saving to: 'garden.jpg'

garden.jpg          100%[==================>]   2.19M  --.-KB/s    in 0.01s   

2024-03-15 01:08:28 (162 MB/s) - 'garden.jpg' saved [2295192/2295192]

janviier-picoctf@webshell:~$ strings garden.jpg | grep pico
Here is a flag "picoCTF{more_than_m33ts_the_3y3eBdBd2cc}"
janviier-picoctf@webshell:~$ 

```

picoCTF{more_than_m33ts_the_3y3eBdBd2cc}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/44