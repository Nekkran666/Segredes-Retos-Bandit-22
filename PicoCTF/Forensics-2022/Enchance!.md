# Enchance!

## Descripcion
Download this image file and find the flag.

-   [Download image file](https://artifacts.picoctf.net/c/137/drawing.flag.svg)

## Pistas
```bash
──(kali㉿kali)-[~/PicoCTF/forensic2022/enchance]
└─$ strings drawing.flag.svg| grep tspan
       id="text3723"><tspan
         id="tspan3748">p </tspan><tspan
         id="tspan3754">i </tspan><tspan
         id="tspan3756">c </tspan><tspan
         id="tspan3758">o </tspan><tspan
         id="tspan3760">C </tspan><tspan
         id="tspan3762">T </tspan><tspan
         id="tspan3764">F { 3 n h 4 n </tspan><tspan
         id="tspan3752">c 3 d _ 2 4 3 7 4 6 7 5 }</tspan></text>

```
picoCTF{3nh4nc3d_24374675}
## Solucion 

## Notas Adicionales

## Referencias