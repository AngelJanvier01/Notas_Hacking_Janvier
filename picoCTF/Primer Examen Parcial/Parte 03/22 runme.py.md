Puntos: 5pts
# Objetivo del Nivel

Run the `runme.py` script to get the flag. Download the script with your browser or with `wget` in the webshell.[Download runme.py Python script](https://artifacts.picoctf.net/c/34/runme.py)`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/34/runme.py
--2024-03-03 05:49:17--  https://artifacts.picoctf.net/c/34/runme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.128, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 270 [application/octet-stream]
Saving to: 'runme.py'

runme.py                                                          100%[=============================================================================================================================================================>]     270  --.-KB/s    in 0s      

2024-03-03 05:49:17 (11.5 MB/s) - 'runme.py' saved [270/270]

janviier-picoctf@webshell:~$ python r
python: can't open file '/home/janviier-picoctf/r': [Errno 2] No such file or directory
janviier-picoctf@webshell:~$ python runme.py 
picoCTF{run_s4n1ty_run}
janviier-picoctf@webshell:~$ 

```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/