# Objetivo del Nivel
The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once
# Datos de Acceso Al Nivel
bandit8 TESKZC0XvTetK0S9xNwm25STk5iWrBvP
# Solución

```bash
bandit8@bandit:~$ cat data.txt | sort | uniq -u
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```

# Notas Adicionales
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Referencias
- [Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
- [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](http://tldp.org/LDP/abs/html/special-chars.html)
- [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)