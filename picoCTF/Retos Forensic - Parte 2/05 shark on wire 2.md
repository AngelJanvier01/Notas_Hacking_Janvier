Puntos: 300pts
# Objetivo del Nivel

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

# Pistas del Nivel

- none
# Solución/Resultado/Flag

```bash
┌──(kali㉿kali)-[~/]
└─$ wireshark capture.pcap  
                                                                             
┌──(kali㉿kali)-[~/]
└─$ cat datos.txt 
No.     Time           Source                Destination           Protocol Length Info
   1104 991.587437     10.0.0.66             10.0.0.1              UDP      60     5000 → 22 Len=5

Frame 1104: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5000, Dst Port: 22
Data (5 bytes)

0000  73 74 61 72 74                                    start

No.     Time           Source                Destination           Protocol Length Info
   1106 993.672341     10.0.0.66             10.0.0.1              UDP      60     5112 → 22 Len=5

Frame 1106: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5112, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1118 1006.227400    10.0.0.66             10.0.0.1              UDP      60     5105 → 22 Len=5

Frame 1118: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5105, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1122 1008.323546    10.0.0.66             10.0.0.1              UDP      60     5099 → 22 Len=5

Frame 1122: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5099, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1124 1010.428768    10.0.0.66             10.0.0.1              UDP      60     5111 → 22 Len=5

Frame 1124: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5111, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1129 1012.535515    10.0.0.66             10.0.0.1              UDP      60     5067 → 22 Len=5

Frame 1129: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5067, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1131 1014.627130    10.0.0.66             10.0.0.1              UDP      60     5084 → 22 Len=5

Frame 1131: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5084, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1133 1016.719657    10.0.0.66             10.0.0.1              UDP      60     5070 → 22 Len=5

Frame 1133: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5070, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1135 1018.807279    10.0.0.66             10.0.0.1              UDP      60     5123 → 22 Len=5

Frame 1135: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5123, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1137 1020.899193    10.0.0.66             10.0.0.1              UDP      60     5112 → 22 Len=5

Frame 1137: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5112, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1139 1022.991480    10.0.0.66             10.0.0.1              UDP      60     5049 → 22 Len=5

Frame 1139: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5049, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1141 1025.083748    10.0.0.66             10.0.0.1              UDP      60     5076 → 22 Len=5

Frame 1141: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5076, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1143 1027.167730    10.0.0.66             10.0.0.1              UDP      60     5076 → 22 Len=5

Frame 1143: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5076, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1145 1029.255106    10.0.0.66             10.0.0.1              UDP      60     5102 → 22 Len=5

Frame 1145: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5102, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1147 1031.334799    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5

Frame 1147: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5051, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1162 1043.850969    10.0.0.66             10.0.0.1              UDP      60     5114 → 22 Len=5

Frame 1162: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5114, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1164 1045.934960    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5

Frame 1164: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5051, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1166 1048.019181    10.0.0.66             10.0.0.1              UDP      60     5100 → 22 Len=5

Frame 1166: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5100, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1172 1054.255069    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5

Frame 1172: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5095, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1178 1060.507360    10.0.0.66             10.0.0.1              UDP      60     5100 → 22 Len=5

Frame 1178: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5100, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1180 1062.619741    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5

Frame 1180: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5097, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1187 1066.779955    10.0.0.66             10.0.0.1              UDP      60     5116 → 22 Len=5

Frame 1187: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5116, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1189 1068.867478    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5

Frame 1189: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5097, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1192 1070.959143    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5

Frame 1192: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5095, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1196 1073.043525    10.0.0.66             10.0.0.1              UDP      60     5118 → 22 Len=5

Frame 1196: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5118, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1199 1075.127069    10.0.0.66             10.0.0.1              UDP      60     5049 → 22 Len=5

Frame 1199: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5049, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1267 1139.786992    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5

Frame 1267: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5097, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1272 1141.870974    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5

Frame 1272: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5095, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1274 1143.955404    10.0.0.66             10.0.0.1              UDP      60     5115 → 22 Len=5

Frame 1274: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5115, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1276 1146.043247    10.0.0.66             10.0.0.1              UDP      60     5116 → 22 Len=5

Frame 1276: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5116, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1284 1154.383039    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5

Frame 1284: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5051, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1286 1156.475039    10.0.0.66             10.0.0.1              UDP      60     5103 → 22 Len=5

Frame 1286: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5103, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1296 1166.882937    10.0.0.66             10.0.0.1              UDP      60     5048 → 22 Len=5

Frame 1296: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5048, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1301 1168.975486    10.0.0.66             10.0.0.1              UDP      60     5125 → 22 Len=5

Frame 1301: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.66, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5125, Dst Port: 22
Data (5 bytes)

0000  61 61 61 61 61                                    aaaaa

No.     Time           Source                Destination           Protocol Length Info
   1303 1171.059146    10.0.0.80             10.0.0.1              UDP      60     5000 → 22 Len=3

Frame 1303: 60 bytes on wire (480 bits), 60 bytes captured (480 bits)
Ethernet II, Src: VMware_b9:02:a9 (00:0c:29:b9:02:a9), Dst: Broadcast (ff:ff:ff:ff:ff:ff)
Internet Protocol Version 4, Src: 10.0.0.80, Dst: 10.0.0.1
User Datagram Protocol, Src Port: 5000, Dst Port: 22
Data (3 bytes)

0000  65 6e 64                                          end
                                                                             
┌──(kali㉿kali)-[~/]
└─$ cat datos.txt | grep UDP
   1104 991.587437     10.0.0.66             10.0.0.1              UDP      60     5000 → 22 Len=5
   1106 993.672341     10.0.0.66             10.0.0.1              UDP      60     5112 → 22 Len=5
   1118 1006.227400    10.0.0.66             10.0.0.1              UDP      60     5105 → 22 Len=5
   1122 1008.323546    10.0.0.66             10.0.0.1              UDP      60     5099 → 22 Len=5
   1124 1010.428768    10.0.0.66             10.0.0.1              UDP      60     5111 → 22 Len=5
   1129 1012.535515    10.0.0.66             10.0.0.1              UDP      60     5067 → 22 Len=5
   1131 1014.627130    10.0.0.66             10.0.0.1              UDP      60     5084 → 22 Len=5
   1133 1016.719657    10.0.0.66             10.0.0.1              UDP      60     5070 → 22 Len=5
   1135 1018.807279    10.0.0.66             10.0.0.1              UDP      60     5123 → 22 Len=5
   1137 1020.899193    10.0.0.66             10.0.0.1              UDP      60     5112 → 22 Len=5
   1139 1022.991480    10.0.0.66             10.0.0.1              UDP      60     5049 → 22 Len=5
   1141 1025.083748    10.0.0.66             10.0.0.1              UDP      60     5076 → 22 Len=5
   1143 1027.167730    10.0.0.66             10.0.0.1              UDP      60     5076 → 22 Len=5
   1145 1029.255106    10.0.0.66             10.0.0.1              UDP      60     5102 → 22 Len=5
   1147 1031.334799    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5
   1162 1043.850969    10.0.0.66             10.0.0.1              UDP      60     5114 → 22 Len=5
   1164 1045.934960    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5
   1166 1048.019181    10.0.0.66             10.0.0.1              UDP      60     5100 → 22 Len=5
   1172 1054.255069    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5
   1178 1060.507360    10.0.0.66             10.0.0.1              UDP      60     5100 → 22 Len=5
   1180 1062.619741    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5
   1187 1066.779955    10.0.0.66             10.0.0.1              UDP      60     5116 → 22 Len=5
   1189 1068.867478    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5
   1192 1070.959143    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5
   1196 1073.043525    10.0.0.66             10.0.0.1              UDP      60     5118 → 22 Len=5
   1199 1075.127069    10.0.0.66             10.0.0.1              UDP      60     5049 → 22 Len=5
   1267 1139.786992    10.0.0.66             10.0.0.1              UDP      60     5097 → 22 Len=5
   1272 1141.870974    10.0.0.66             10.0.0.1              UDP      60     5095 → 22 Len=5
   1274 1143.955404    10.0.0.66             10.0.0.1              UDP      60     5115 → 22 Len=5
   1276 1146.043247    10.0.0.66             10.0.0.1              UDP      60     5116 → 22 Len=5
   1284 1154.383039    10.0.0.66             10.0.0.1              UDP      60     5051 → 22 Len=5
   1286 1156.475039    10.0.0.66             10.0.0.1              UDP      60     5103 → 22 Len=5
   1296 1166.882937    10.0.0.66             10.0.0.1              UDP      60     5048 → 22 Len=5
   1301 1168.975486    10.0.0.66             10.0.0.1              UDP      60     5125 → 22 Len=5
   1303 1171.059146    10.0.0.80             10.0.0.1              UDP      60     5000 → 22 Len=3
                                                                             
┌──(kali㉿kali)-[~/]
└─$ cat datos.txt | grep UDP  | awk '{print $7}' | cut -c2- | grep -v 000
112
105
099
111
067
084
070
123
112
049
076
076
102
051
114
051
100
095
100
097
116
097
095
118
049
097
095
115
116
051
103
048
125

picoCTF{p1LLf3r3d_data_v1a_st3g0}
```

picoCTF{p1LLf3r3d_data_v1a_st3g0}
# Notas Adicionales
# Referencias

https://play.picoctf.org/practice/challenge/84