# PicoCTF

## Descripcion
There's something in the [building](https://jupiter.challenges.picoctf.org/static/011955b303f293d60c8116e6a4c5c84f/buildings.png). Can you retrieve the flag?

## Pistas
1. There is data encoded somewhere... there might be an online decoder.

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/forensic2019/wlw]
└─$ zsteg -a buildings.png | grep pico  
```

picoCTF{h1d1ng_1n_th3_b1t5}

## Notas Adicionales

## Referencias