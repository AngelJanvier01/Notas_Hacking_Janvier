Puntos: 5pts
# Objetivo del Nivel

Our flag printing service has started glitching!`$ nc saturn.picoctf.net 55826`
# Pistas del Nivel
- 
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ nc saturn.picoctf.net 55826
'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'



On CyberChef

0x390x630x340x320x610x340x350x64

FROM HEX:

9c42a45d

picoCTF{gl17ch_m3_n07_9c42a45d}
```
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/