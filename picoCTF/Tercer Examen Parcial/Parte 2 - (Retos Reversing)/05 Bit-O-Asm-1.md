Puntos: 100pts
# Objetivo del Nivel

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/509/disassembler-dump0_a.txt).
# Pistas del Nivel
- As with most assembly, there is a lot of noise in the instruction dump. Find the one line that pertains to this question and don't second guess yourself!
# Solución/Resultado/Flag

```bash

En el archivo de volcado de ensamblador hay una instrucción
`mov eax,0x30`
lo que significa que estamos almacenando el valor de 0x30 en el registro eax.
0x30 en hexadecimal es 48 en decimal:

picoCTF{48}

```

picoCTF{48}-

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/