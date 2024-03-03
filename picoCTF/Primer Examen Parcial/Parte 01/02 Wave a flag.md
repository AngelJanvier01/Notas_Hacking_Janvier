Puntos: 5pts
# Objetivo del Nivel

Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/a00f554b16385d9970dae424f66ee1ab/warm) has extraordinarily helpful information...
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/a00f554b16385d9970dae424f66ee1ab/warm
--2024-03-03 04:37:15--  https://mercury.picoctf.net/static/a00f554b16385d9970dae424f66ee1ab/warm
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 10936 (11K) [application/octet-stream]
Saving to: 'warm'

warm                                                              100%[=============================================================================================================================================================>]  10.68K  --.-KB/s    in 0s      

2024-03-03 04:37:16 (281 MB/s) - 'warm' saved [10936/10936]

janviier-picoctf@webshell:~$ ls
README.txt  flag  warm
janviier-picoctf@webshell:~$ chmod +x warm
janviier-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
janviier-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_18788aaa}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/