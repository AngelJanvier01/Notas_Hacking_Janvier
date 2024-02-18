# Objetivo del Nivel
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data
# Datos de Acceso Al Nivel
bandit11 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
# Solución

```bash
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi
bandit11@bandit:~$ python3
Python 3.10.12 (main, Jun 12 2023, 06:26:28) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import codecs
>>> codecs.decode('Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi','rot13')
'The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv'
```

# Notas Adicionales
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Referencias
- [Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
- [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](http://tldp.org/LDP/abs/html/special-chars.html)
- [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)
- [Base64 on Wikipedia](https://en.wikipedia.org/wiki/Base64)
- [Rot13 on Wikipedia](https://en.wikipedia.org/wiki/Rot13)