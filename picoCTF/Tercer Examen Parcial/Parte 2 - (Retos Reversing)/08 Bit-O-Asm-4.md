Puntos: 100pts
# Objetivo del Nivel

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Download the assembly dump [here](https://artifacts.picoctf.net/c/511/disassembler-dump0_d.txt).
# Pistas del Nivel
- Don't tell anyone I told you this, but you can solve this problem without understanding the compare/jump relationship.
- Of course, if you're really good, you'll only need one attempt to solve this problem.
# Solución/Resultado/Flag

```bash

En el archivo de volcado de ensamblador hay las siguientes instrucciones:

<+15>:    mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    cmp    DWORD PTR [rbp-0x4],0x2710
<+29>:    jle    0x55555555514e <main+37>
<+31>:    sub    DWORD PTR [rbp-0x4],0x65
<+35>:    jmp    0x555555555152 <main+41>
<+37>:    add    DWORD PTR [rbp-0x4],0x65
<+41>:    mov    eax,DWORD PTR [rbp-0x4]

Esto es lo que ejecuta la CPU:

<+15>:  Almacenar 0x9fe1a en la memoria apuntada por [rbp-0x4]
<+22>:  Comparar [rbp-0x4] con 0x2710
<+29>:  Saltar a la instrucción en <+37> si [rbp-0x4] es menor o igual a 0x2710 (NO lo es)
<+31>:  Restar 0x65 de [rbp-0x4] y almacenar el resultado en [rbp-0x4]
<+35>:  Saltar a <+41>
<+37>:  [NO EJECUTADO]
<+41>:  Almacenar el valor apuntado por [rbp-0x4] en el registro eax

Después de todas las operaciones y la conversión de hexadecimal, obtenemos el número decimal y nuestra bandera:

picoCTF{654773}
```


picoCTF{654773}

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/