Puntos: 20pts
# Objetivo del Nivel

I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled2.png)
# Pistas del Nivel
- [https://en.wikipedia.org/wiki/Visual_cryptography](https://en.wikipedia.org/wiki/Visual_cryptography)
- Think of different ways you can "stack" images
# Solución/Resultado/Flag

```bash
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ ls
atbash.jpg  code.py  message.txt
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ wget https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled1.png
--2024-04-16 13:04:02--  https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled1.png
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 197171 (193K) [application/octet-stream]
Saving to: ‘scrambled1.png’

scrambled1.png                                       100%[=====================================================================================================================>] 192.55K   237KB/s    in 0.8s

2024-04-16 13:04:12 (237 KB/s) - ‘scrambled1.png’ saved [197171/197171]

janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ wget https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled2.png
--2024-04-16 13:04:31--  https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled2.png
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 197173 (193K) [application/octet-stream]
Saving to: ‘scrambled2.png’

scrambled2.png                                       100%[=====================================================================================================================>] 192.55K   216KB/s    in 0.9s

2024-04-16 13:04:40 (216 KB/s) - ‘scrambled2.png’ saved [197173/197173]

janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python3 code
code.py          codeimaggggg.py
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python3 codeimaggggg.py
Traceback (most recent call last):
  File "/home/janviier/PICOCTFJANVIER/codeimaggggg.py", line 1, in <module>
    from PIL import Image
ModuleNotFoundError: No module named 'PIL'
janviier@PAVILION-Janvier:~/PICOCTFJANVIER$ python3
Python 3.10.12 (main, Jun 11 2023, 05:26:28) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> pip install PIL
  File "<stdin>", line 1
    pip install PIL
        ^^^^^^^
SyntaxError: invalid syntax
>>> pip install PIL
  File "<stdin>", line 1
    pip install PIL
        ^^^^^^^
SyntaxError: invalid syntax
>>> pip PIL
  File "<stdin>", line 1
    pip PIL
        ^^^
SyntaxError: invalid syntax
>>> pip install pillow
  File "<stdin>", line 1
    pip install pillow
        ^^^^^^^
SyntaxError: invalid syntax
>



from PIL import Image
import numpy as np
import os

file_names = ["scrambled1.png", "scrambled2.png"]
img_data = [np.asarray(Image.open(f'{name}')) for name in file_names]

data = img_data[0].copy() + img_data[1].copy()

new_image = Image.fromarray(data)
new_image.save("out.png", "PNG")

picoCTF{0542dc1d}

```

picoCTF{0542dc1d}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/