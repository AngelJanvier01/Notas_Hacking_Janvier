Puntos: 20pts
# Objetivo del Nivel

In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/38f30029ab93478310e906d3d084a4c1/values)
# Pistas del Nivel
- Bits are expensive, I used only a little bit over 100 to save money
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~/picoabrilctf$ cat values 
Decrypt my super sick RSA:
c: 240986837130071017759137533082982207147971245672412893755780400885108149004760496
n: 831416828080417866340504968188990032810316193533653516022175784399720141076262857
e: 65537janviier-picoctf@webshell:~/picoabrilctf$ ^C
janviier-picoctf@webshell:~/picoabrilctf$ ^C
janviier-picoctf@webshell:~/picoabrilctf$ python
Python 3.10.12 (main, Nov 20 2023, 15:14:05) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> p = 1593021310640923782355996681284584012117
>>> 
>>> q = 521911930824021492581321351826927897005221
>>> n = p*q
>>> e = 65537
>>> c = 
KeyboardInterrupt
>>> c = 240986837130071017759137533082982207147971245672412893755780400885108149004760496
>>> tn = (p-1)*(q-1)
>>> d = pow(e, -1, tn)
>>> 
>>> m = pow(c, d, n)
>>> 
>>> m
13016382529449106065927291425342535437996222135352905256639592405461024281868413
>>> bytes.fromhex( hex(m)[2:] )
b'picoCTF{sma11_N_n0_g0od_23540368}'
>>> 
```

picoCTF{sma11_N_n0_g0od_23540368}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/