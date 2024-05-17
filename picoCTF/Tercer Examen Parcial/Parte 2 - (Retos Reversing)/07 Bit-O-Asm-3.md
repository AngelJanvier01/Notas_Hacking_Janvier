Puntos: 100pts
# Objetivo del Nivel

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/530/disassembler-dump0_c.txt).
# Pistas del Nivel
- Not everything in this disassembly listing is optimal.
# Solución/Resultado/Flag

```bash

En el archivo de volcado de ensamblador hay las siguientes instrucciones:

<+15>:    mov    DWORD PTR [rbp-0xc],0x9fe1a
<+22>:    mov    DWORD PTR [rbp-0x8],0x4
<+29>:    mov    eax,DWORD PTR [rbp-0xc]
<+32>:    imul   eax,DWORD PTR [rbp-0x8]
<+36>:    add    eax,0x1f5
<+41>:    mov    DWORD PTR [rbp-0x4],eax
<+44>:    mov    eax,DWORD PTR [rbp-0x4]

Esto es lo que ejecuta la CPU:

<+15>:    El valor DWORD 654874 se almacena en la ubicación de memoria apuntada por [rbp-0xc]
<+22>:    El valor DWORD 4 se almacena en la ubicación de memoria apuntada por [rbp-0x8]
<+29>:    El valor almacenado en la ubicación de memoria apuntada por [rbp-0xc] (654874) se almacena en el registro eax
<+32>:    El valor almacenado en el registro eax se multiplica con el valor almacenado en la ubicación de memoria apuntada por [rbp-0x8] (4) y el resultado se almacena en el registro eax
<+36>:    Se suma el valor 501 al valor almacenado en el registro eax y el resultado se almacena en el registro eax
<+41>:    El valor almacenado en el registro eax se almacena en la ubicación de memoria apuntada por [rbp-0x4]
<+44>:    El valor en la ubicación de memoria apuntada por [rbp-0x4] se almacena en el registro eax

Por lo tanto, la bandera es:

picoCTF{2619997}

```

picoCTF{2619997}

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/