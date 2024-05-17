Puntos: 100pts
# Objetivo del Nivel

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).
# Pistas del Nivel
- `PTR`'s or 'pointers', reference a location in memory where values can be stored.
# Solución/Resultado/Flag

```bash

En el archivo de volcado de ensamblador hay las siguientes dos instrucciones:

<+15>:    mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    mov    eax,DWORD PTR [rbp-0x4]

Esto significa que estamos almacenando el valor DWORD 0x9fe1a en la ubicación de memoria apuntada por [rbp-0x4] (instrucción 1) y almacenando ese valor en el registro eax (instrucción 2).

0x9fe1a en hexadecimal es 654874 en decimal:

picoCTF{654874}

```

picoCTF{654874}

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/