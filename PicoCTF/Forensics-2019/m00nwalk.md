# PicoCTF

## Descripcion
Decode this [message](https://jupiter.challenges.picoctf.org/static/d6fcea5e3c6433680ea4f914e24fab61/message.wav) from the moon.

## Pistas
1. How did pictures from the moon landing get sent back to Earth?
2. How did pictures from the moon landing get sent back to Earth?

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/forensic2019/moon]
└─$ sstv -d message.wav -o result.png        
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [#################################################################################] 100%
[sstv] Drawing image data...
[sstv] ...Don
```
picoCTF{beep_boop_im_in_space}

## Notas Adicionales

## Referencias