Puntos: 50pts
# Objetivo del Nivel

This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?

# Pistas del Nivel

- How do operating systems know what kind of file it is? (It's not just the ending!
- Make sure to submit the flag as picoCTF{XXXXX}
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt
--2024-03-15 01:12:03--  https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9984 (9.8K) [application/octet-stream]
Saving to: 'flag.txt'

flag.txt                              100%[=========================================================================>]   9.75K  --.-KB/s    in 0s      

2024-03-15 01:12:03 (300 MB/s) - 'flag.txt' saved [9984/9984]

janviier-picoctf@webshell:~$ file flag.txt 
flag.txt: PNG image data, 1697 x 608, 8-bit/color RGB, non-interlaced
janviier-picoctf@webshell:~$ mv flag.txt flag.png
janviier-picoctf@webshell:~$ open flag.png
Error: no "view" rule for type "image/png" passed its test case
       (for more information, add "--debug=1" on the command line)
janviier-picoctf@webshell:~$ 
janviier-picoctf@webshell:~$ open flag.png
picoCTF{now_you_know_about_extensions}
```

picoCTF{now_you_know_about_extensions}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/52