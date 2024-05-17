Puntos: 20pts
# Objetivo del Nivel

I wonder what this really is... [enc](https://mercury.picoctf.net/static/0d3145dafdc4fbcf01891912eb6c0968/enc) `''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])`
# Pistas del Nivel
- You may find some decoders online
# Solución/Resultado/Flag

```bash

janviier@Janvier-DeskTop:~/picotercerex/pt2ex$ wget https://mercury.picoctf.net/static/0d3145dafdc4fbcf01891912eb6c0968/enc
--2024-05-16 20:51:03--  https://mercury.picoctf.net/static/0d3145dafdc4fbcf01891912eb6c0968/enc
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 57 [application/octet-stream]
Saving to: ‘enc’

enc                           100%[=================================================>]      57  --.-KB/s    in 0s

2024-05-16 20:51:03 (27.2 MB/s) - ‘enc’ saved [57/57]

janviier@Janvier-DeskTop:~/picotercerex/pt2ex$ ls
enc
janviier@Janvier-DeskTop:~/picotercerex/pt2ex$ cat enc
灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸弲㘶㠴挲ぽjanviier@Janvier-DeskTop:~/picotercerex/pt2ex$ python3 script.py enc
  File "/home/janviier/picotercerex/pt2ex/script.py", line 9
    print("Flag: " + flag)s
                          ^
SyntaxError: invalid syntax
janviier@Janvier-DeskTop:~/picotercerex/pt2ex$ python3 script.py enc
Flag: picoCTF{16_bits_inst34d_of_8_26684c20}
janviier@Janvier-DeskTop:~/picotercerex/pt2ex$

```

picoCTF{16_bits_inst34d_of_8_26684c20}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/