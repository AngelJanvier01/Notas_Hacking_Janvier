# Objetivo del Nivel
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.
# Datos de Acceso Al Nivel
bandit9 EN632PlfYiZbn3PhVK3XOGSlNInNE00t
# Solución

```bash
bandit9@bandit:~$ strings  data.txt | grep ==
x]T========== theG)"
========== passwordk^
========== is
========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
bandit9@bandit:~$
```

# Notas Adicionales
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd
# Referencias
- [Google Search for “dashed filename”](https://www.google.com/search?q=dashed+filename)
- [Advanced Bash-scripting Guide - Chapter 3 - Special Characters](http://tldp.org/LDP/abs/html/special-chars.html)
- [Piping and Redirection](https://ryanstutorials.net/linuxtutorial/piping.php)