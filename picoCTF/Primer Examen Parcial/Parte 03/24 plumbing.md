Puntos: 5pts
# Objetivo del Nivel

Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291 > file
wc file
janviier-picoctf@webshell:~$ wc file
 10001  62040 288139 file
janviier-picoctf@webshell:~$ cat file | grep pico
picoCTF{digital_plumb3r_ea8bfec7}
janviier-picoctf@webshell:~$ 

```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/