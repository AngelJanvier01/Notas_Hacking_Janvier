Puntos: 20pts
# Objetivo del Nivel

Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:47967/](http://mercury.picoctf.net:47967/)

# Pistas del Nivel

- Maybe you have more than 2 choices
- Check out tools like Burpsuite to modify your requests and look at the responses
# Solución/Resultado/Flag

```bash
==========================================================================

janviier-picoctf@webshell:~$ curl -I HEAD -i http://mercury.picoctf.net:47967/index.php
curl: (6) Could not resolve host: HEAD
HTTP/1.1 200 OK
flag: picoCTF{r3j3ct_th3_du4l1ty_cca66bd3}
Content-type: text/html; charset=UTF-8

janviier-picoctf@webshell:~$ 

janviier-picoctf@webshell:~$ 

```

picoCTF{r3j3ct_th3_du4l1ty_cca66bd3}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/132