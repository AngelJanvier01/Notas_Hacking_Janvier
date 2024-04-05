Puntos: 100pts
# Objetivo del Nivel

Download the packet capture file and use packet analysis software to find the flag.

- [Download packet capture](https://artifacts.picoctf.net/c/196/network-dump.flag.pcap)
# Pistas del Nivel
- Wireshark, if you can install and use it, is probably the most beginner friendly packet analysis software product.
# Solución/Resultado/Flag

```bash
Obtener el archivo (wget)

Crear una instancia de captura de paquetes

seguir la trasmision de TCP

el primer stream contiene la bandera

picoCTF{p4ck37_5h4rk_01b0a0d6}
```

picoCTF{p4ck37_5h4rk_01b0a0d6}
# Notas Adicionales

Tags:

AUTHOR:
# Referencias

https://play.picoctf.org/practice/challenge/