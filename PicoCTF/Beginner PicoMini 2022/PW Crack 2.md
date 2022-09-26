# PW Crack 2 

## Descripcion
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/17/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level2.flag.txt.enc) in the same directory too.

## Pistas
1. Does that encoding look familiar?
2. The `str_xor` function does not need to be reverse engineered for this challenge.

## Solucion 
```bash
┌──(kali㉿kali)-[~/Downloads]
└─$ nano level2.py
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3          
Python 3.10.5 (main, Jun  8 2022, 09:26:22) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))
4ec9
>>> 
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 level2.py
Please enter correct password for flag: 4ec9
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_9701e681}
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]

```


## Notas Adicionales

## Referencias