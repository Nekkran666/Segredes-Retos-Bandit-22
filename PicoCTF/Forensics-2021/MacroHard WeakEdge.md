# MacroHard WeakEdge

## Descripcion
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/9a7436948cc502e9cacf5bc84d2cccb5/Forensics is fun.pptm)

## Pistas

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/forensic2021/Macro]
└─$ echo "Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q" | tr -d " " | base64 -d 
flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}base64: invalid input

```

## Notas Adicionales

## Referencias