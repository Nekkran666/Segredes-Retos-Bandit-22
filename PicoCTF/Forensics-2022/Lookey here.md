# Lookey here

## Descripcion
Attackers have hidden information in a very large mass of data in the past, maybe they are still doing it. Download the data [here](https://artifacts.picoctf.net/c/295/anthem.flag.txt).

## Pistas
1. Download the file and search for the flag based on the known prefix.
## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/forensic2022/lkhr]
└─$ cat anthem.flag.txt | grep pico
      we think that the men of picoCTF{gr3p_15_@w3s0m3_58f5c024}
                                                                    
```

## Notas Adicionales

## Referencias