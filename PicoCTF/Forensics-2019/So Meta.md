# PicoCTF

## Descripcion
Find the flag in this [picture](https://jupiter.challenges.picoctf.org/static/00efdf2961da1e21470ffc0d496c3cc2/pico_img.png).

## Pistas
1. What does meta mean in the context of files?
2. Ever heard of metadata?

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/forensic2019/soMeta]
└─$ exiftool pico_img.png -Artist
Artist                          : picoCTF{s0_m3ta_fec06741}

```

## Notas Adicionales

## Referencias