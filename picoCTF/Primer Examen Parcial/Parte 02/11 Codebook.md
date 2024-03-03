Puntos: 5pts
# Objetivo del Nivel

Run the Python script `code.py` in the same directory as `codebook.txt`.

- [Download code.py](https://artifacts.picoctf.net/c/1/code.py)
- [Download codebook.txt](https://artifacts.picoctf.net/c/1/codebook.txt)
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/1/code.py
--2024-03-03 05:18:22--  https://artifacts.picoctf.net/c/1/code.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.43, 3.160.22.128, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1278 (1.2K) [application/octet-stream]
Saving to: 'code.py'

code.py                                                           100%[=============================================================================================================================================================>]   1.25K  --.-KB/s    in 0s      

2024-03-03 05:18:22 (416 MB/s) - 'code.py' saved [1278/1278]

janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/1/codebook.txt
--2024-03-03 05:18:31--  https://artifacts.picoctf.net/c/1/codebook.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.16, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 27 [application/octet-stream]
Saving to: 'codebook.txt'

codebook.txt                                                      100%[=============================================================================================================================================================>]      27  --.-KB/s    in 0s      

2024-03-03 05:18:31 (10.5 MB/s) - 'codebook.txt' saved [27/27]

janviier-picoctf@webshell:~$ python code.py 
picoCTF{c0d3b00k_455157_d9aa2df2}
janviier-picoctf@webshell:~$ ^C
janviier-picoctf@webshell:~$ 
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/