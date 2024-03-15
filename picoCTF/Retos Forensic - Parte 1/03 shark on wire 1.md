Puntos: 150pts
# Objetivo del Nivel

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap). Recover the flag.

# Pistas del Nivel

- Try using a tool like Wireshark
- What are streams?
# Solución/Resultado/Flag

```bash
janviier-picoctf@webshell:~$ ls
Addadshashanammu      code.py       file       flag        index.html           level2.flag.txt.enc  level3.hash.bin  static
Addadshashanammu.zip  codebook.txt  fixme1.py  flag.png    level1.flag.txt.enc  level2.py            level3.py        strings
README.txt            convertme.py  fixme2.py  garden.jpg  level1.py            level3.flag.txt.enc  runme.py         warm
janviier-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap
--2024-03-15 01:16:22--  https://jupiter.challenges.picoctf.org/static/483e50268fe7e015c49caf51a69063d0/capture.pcap
Resolving jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)... 3.131.60.8
Connecting to jupiter.challenges.picoctf.org (jupiter.challenges.picoctf.org)|3.131.60.8|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 239455 (234K) [application/octet-stream]
Saving to: 'capture.pcap'

capture.pcap                          100%[=========================================================================>] 233.84K  --.-KB/s    in 0.004s  

2024-03-15 01:16:22 (53.2 MB/s) - 'capture.pcap' saved [239455/239455]

janviier-picoctf@webshell:~$ wireshark
janviier-picoctf@webshell:~$ open capture.pcap
picoCTF{StaT31355_636f6e6e}
```

picoCTF{StaT31355_636f6e6e}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/30