# Objetivo del Nivel
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data
# Datos de Acceso Al Nivel
bandit10 G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
# Solución

```bash
bandit10@bandit:~$ cat data.txt | base64 -d
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
```

# Notas Adicionales
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Referencias
- [Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
- [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](http://tldp.org/LDP/abs/html/special-chars.html)
- [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)
- [Base64 on Wikipedia](https://en.wikipedia.org/wiki/Base64)