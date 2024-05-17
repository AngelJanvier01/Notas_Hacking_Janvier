Puntos: 100pts
# Objetivo del Nivel

Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`.Disassemble [this](https://artifacts.picoctf.net/c/512/debugger0_a).
# Pistas del Nivel
- gdb is a very good debugger to use for this problem and many others!
- `main` is actually a recognized symbol that can be used with gdb commands.
# Solución/Resultado/Flag

```bash
Descarga el binario y ejecuta gdb con 'gdb debugger0_a'.
Desensambla la función main() con 'disassemble main' y obtendrás el volcado:

   0x0000000000001129 <+0>:     endbr64
   0x000000000000112d <+4>:     push   %rbp
   0x000000000000112e <+5>:     mov    %rsp,%rbp
   0x0000000000001131 <+8>:     mov    %edi,-0x4(%rbp)
   0x0000000000001134 <+11>:    mov    %rsi,-0x10(%rbp)
   0x0000000000001138 <+15>:    mov    $0x86342,%eax
   0x000000000000113d <+20>:    pop    %rbp
   0x000000000000113e <+21>:    ret

Como puedes ver, en <+15> el valor 0x86342 se almacena en el registro eax (recuerda, esta es la sintaxis de AT&T, por lo tanto, ¡los operandos están invertidos!).

Así que la bandera es:

picoCTF{549698}
```

picoCTF{549698}

# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/