# GLory of the Garden

## Descripcion
This [garden](https://jupiter.challenges.picoctf.org/static/43c4743b3946f427e883f6b286f47467/garden.jpg) contains more than it seems.

## Pistas
1. What is a hex editor?

## Solucion 
```bash                                      
┌──(kali㉿kali)-[~/PicoCTF/forensic2019/goOfGa]
└─$ strings -n 13 garden.jpg | grep picoCTF
Here is a flag "picoCTF{more_than_m33ts_the_3y3657BaB2C}"
```


## Notas Adicionales

## Referencias