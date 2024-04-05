Puntos: 100pts
# Objetivo del Nivel

The developer of this website mistakenly left an important artifact in the website source, can you find it?
The website is [here](http://saturn.picoctf.net:59405/)
# Pistas del Nivel
- How could you mirror the website on your local machine so you could use more powerful tools for searching?
# Solución/Resultado/Flag

```bash
me puse a buscar en todo el source code la bandera pero es mucho texto asi que descargare la pag  y
le hare todos los trucos:

janviier-picoctf@webshell:~/saturn.picoctf.net:59405$ ls
css  images  index.html  js
janviier-picoctf@webshell:~/saturn.picoctf.net:59405$ grep -r pico
css/style.css:/** banner_main picoCTF{1nsp3ti0n_0f_w3bpag3s_8de925a7} **/
janviier-picoctf@webshell:~/saturn.picoctf.net:59405$ 

```

picoCTF{1nsp3ti0n_0f_w3bpag3s_8de925a7}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/