# PicoCTF

## Descripcion
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.

## Pistas
1. Try using a tool like Wireshark.
2. How can you decrypt the TLS stream?

## Solucion 
con ayuda de wireshark se desencriptan los paquetes con la llave que nos dieron, con lo cual nos damos cuenta que hay una imagen que podemos descargar, la descargamos y nos permite encontrar la llave con un strings en consola. 

picoCTF{honey.roasted.peanuts}


## Notas Adicionales

## Referencias