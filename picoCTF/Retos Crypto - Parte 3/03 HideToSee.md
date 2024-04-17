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
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ ls
code.py  message.txt
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ wget https://artifacts.picoctf.net/c/235/atbash.jpg
--2024-04-16 12:55:30--  https://artifacts.picoctf.net/c/235/atbash.jpg
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.55.61, 3.161.55.64, 3.161.55.100, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.55.61|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 51499 (50K) [application/octet-stream]
Saving to: ‘atbash.jpg’

atbash.jpg                                           100%[=====================================================================================================================>]  50.29K  --.-KB/s    in 0.02s

2024-04-16 12:55:38 (2.18 MB/s) - ‘atbash.jpg’ saved [51499/51499]

janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ ls
atbash.jpg  code.py  message.txt
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ sudo apt-get install steghide -y
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
E: Unable to locate package steghide
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ steguide
Command 'steguide' not found, did you mean:
  command 'steghide' from deb steghide (0.5.1-15)
Try: sudo apt install <deb name>
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ sudo apt install steghide
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
E: Unable to locate package steghide
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$

https://futureboy.us/stegano/decinput.html

krxlXGU{zgyzhs_xizxp_92533667} krxlXGU{zgyzhs_xizxp_92533667} krxlXGU{zgyzhs_xizxp_92533667}

https://www.dcode.fr/atbash-cipher

picoCTF{atbash_crack_92533667} picoCTF{atbash_crack_92533667} picoCTF{atbash_crack_92533667}
```

picoCTF{atbash_crack_92533667}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/