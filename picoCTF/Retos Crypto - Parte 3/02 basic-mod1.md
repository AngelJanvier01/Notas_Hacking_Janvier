Puntos: 20pts
# Objetivo del Nivel

We found this weird message being passed around on the servers, we think we have a working decryption scheme.
Download the message here.
Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore.
Wrap your decrypted message in the picoCTF flag format (i.e. picoCTF{decrypted_message})
# Pistas del Nivel
- Do you know what `mod 37` means?
- `mod 37` means modulo 37. It gives the remainder of a number after being divided by 37.
# Solución/Resultado/Flag

```bash
janviier@PAVILION-Janvier:~$ wget https://artifacts.picoctf.net/c/128/message.txt
--2024-04-16 12:34:51--  https://artifacts.picoctf.net/c/128/message.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.55.61, 3.161.55.64, 3.161.55.26, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.55.61|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 84 [application/octet-stream]
Saving to: ‘message.txt’

message.txt                                                 100%[========================================================================================================================================>]      84  --.-KB/s    in 0s

2024-04-16 12:35:13 (2.37 MB/s) - ‘message.txt’ saved [84/84]

janviier@PAVILION-Janvier:~$ cat message.txt
165 248 94 346 299 73 198 221 313 137 205 87 336 110 186 69 223 213 216 216 177 138 janviier@PAVILION-Janvier:~$ ls
message.txt  values
janviier@PAVILION-Janvier:~$ dir
message.txt  values
janviier@PAVILION-Janvier:~$ mkdir PICOCTFJANVIER
janviier@PAVILION-Janvier:~$ wget https://artifacts.picoctf.net/c/128/message.txt
--2024-04-16 12:38:25--  https://artifacts.picoctf.net/c/128/message.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.55.100, 3.161.55.26, 3.161.55.64, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.55.100|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 84 [application/octet-stream]
Saving to: ‘message.txt.1’

message.txt.1                                               100%[========================================================================================================================================>]      84  --.-KB/s    in 0.006s

2024-04-16 12:38:33 (12.8 KB/s) - ‘message.txt.1’ saved [84/84]

janviier@PAVILION-Janvier:~$ ls
PICOCTFJANVIER  message.txt  message.txt.1  values
janviier@PAVILION-Janvier:~$ ls
PICOCTFJANVIER  message.txt.1  values
janviier@PAVILION-Janvier:~$ ls PICO
ls: cannot access 'PICO': No such file or directory
janviier@PAVILION-Janvier:~$ ls PICOCTFJANVIER/
message.txt
janviier@PAVILION-Janvier:~$ cd PICOCTFJANVIER/
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ LS
LS: command not found
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ ls
message.txt
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ cat message.txt
165 248 94 346 299 73 198 221 313 137 205 87 336 110 186 69 223 213 216 216 177 138 janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ ls
code.py  message.txt
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python code.py
Command 'python' not found, did you mean:
  command 'python3' from deb python3
  command 'python' from deb python-is-python3
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python
Command 'python' not found, did you mean:
  command 'python3' from deb python3
  command 'python' from deb python-is-python3
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python3 code.py
[17, 26, 20, 13, 3, 36, 13, 36, 17, 26, 20, 13, 3, 36, 1, 32, 1, 28, 31, 31, 29, 27]
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$

A: 0
B: 1
C: 2
D: 3
E: 4
F: 5
G: 6
H: 7
I: 8
J: 9
K: 10
L: 11
M: 12
N: 13
O: 14
P: 15
Q: 16
R: 17
S: 18
T: 19
U: 20
V: 21
W: 22
X: 23
Y: 24
Z: 25
0: 26
1: 27
2: 28
3: 29
4: 30
5: 31
6: 32
7: 33
8: 34
9: 35
_: 36

osea que, al convertirlo queda:

[17, 26, 20, 13, 3, 36, 13, 36, 17, 26, 20, 13, 3, 36, 1, 32, 1, ,,,28, 31, 31, 29, 27]
	R0UND_N_R0UND_A_B6B25531
	R0UND N R0UND B6B25531
```

picoCTF{R0UND_N_R0UND_B6B25531}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/