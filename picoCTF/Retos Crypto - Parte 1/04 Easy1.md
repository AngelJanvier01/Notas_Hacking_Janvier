Puntos: 100pts
# Objetivo del Nivel

The one time pad can be cryptographically secure, but not when you know the key. Can you solve this? We've given you the encrypted flag, key, and a table to help `UFJKXQZQUNB` with the key of `SOLVECRYPTO`. Can you use this [table](https://jupiter.challenges.picoctf.org/static/1fd21547c154c678d2dab145c29f1d79/table.txt) to solve it?.
# Pistas del Nivel
- Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.
- Please use all caps for the message.
# Solución/Resultado/Flag

```bash
Una clave y una tabla de doble entrada nos dan pistas inmediatas sobre uno de los métodos de cifrado más comunes: el cifrado Vigenère. Aunque hay formas de descifrar mensajes con este cifrado manualmente (usando la tabla en el archivo de texto dado), es mucho más fácil resolverlo con una herramienta en línea como [DCOde]https://www.dcode.fr/vigenere-cipher.

picoCTF{CRYPTOISFUN}
```

picoCTF{CRYPTOISFUN}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/