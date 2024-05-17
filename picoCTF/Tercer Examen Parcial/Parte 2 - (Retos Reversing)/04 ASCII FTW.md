Puntos: 100pts
# Objetivo del Nivel

This program has constructed the flag using hex ascii values. Identify the flag text by disassembling the program.You can download the file from [here](https://artifacts.picoctf.net/c/508/asciiftw).
# Pistas del Nivel
- The combined range of hex-ascii for English alphabets and numerical digits is from 30 to 7A.
- Online hex-ascii converters can be helpful.
# Solución/Resultado/Flag

```bash

He descargado un archivo binario y lo abrí en Ghidra. En la función main() se declaran 31 variables en la pila, cada una con un valor hexadecimal asignado:

0x70 0x69 0x63 0x6f 0x43 0x54 0x46 0x7b 0x41 0x53 0x43 0x49 0x49 0x5f 0x49 0x53 0x5f 0x45 0x41 0x53 0x59 0x5f 0x37 0x42 0x43 0x44 0x39 0x37 0x31 0x44 0x7d

Con la conversión de hexadecimal a ASCII obtienes la bandera:

picoCTF{ASCII_IS_EASY_7BCD971D}
```

picoCTF{ASCII_IS_EASY_7BCD971D}

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/