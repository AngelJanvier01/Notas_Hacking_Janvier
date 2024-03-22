Puntos: 250pts
# Objetivo del Nivel

Decode this [message](https://jupiter.challenges.picoctf.org/static/14393e18d98fedbaedbc28896d7ef31a/message.wav) from the moon.

# Pistas del Nivel

- How did pictures from the moon landing get sent back to Earth?
- What is the CMU mascot?, that might help select a RX option
# Solución/Resultado/Flag

```bash
instalar sstv para decodificar el audio a imagen 

sstv -d ~/Desktop/pico/message.wav  -o ~/Desktop/pico/res.jpg

haciendo esto obtenemos una imagen con la bandera 

┌──(kali㉿kali)-[~/]
└─$ sstv -d message.wav img.jpg     
usage: sstv [-h] [-d AUDIO_FILE] [-o OUTPUT_FILE] [-s SKIP] [-V]
            [--list-modes] [--list-audio-formats] [--list-image-formats]
sstv: error: unrecognized arguments: img.jpg
                                                                             
┌──(kali㉿kali)-[~/]
└─$ sstv -d message.wav -o img.jpg
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [###########################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!
                                                                             
┌──(kali㉿kali)-[~/]
└─$ open img.jpg

picoCTF{beep_boop_im_in_space}
```

picoCTF{beep_boop_im_in_space}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/30