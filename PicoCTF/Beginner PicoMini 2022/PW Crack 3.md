# PW Crack 3

## Descripcion
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/24/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/24/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/24/level3.hash.bin) in the same directory too. There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

## Pistas
1. To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
2.  To exit `bvi` type `:q` and press enter.
3. The `str_xor` function does not need to be reverse engineered for this challenge.

## Solucion 
```bash
┌──(kali㉿kali)-[~/Downloads]
└─$ nano level3.py    
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 level3.py
Please enter correct password for flag: f09e
That password is incorrect
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 level3.py
Please enter correct password for flag: 4dcf
That password is incorrect
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 level3.py
Please enter correct password for flag: 87ab
That password is incorrect
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 level3.py
Please enter correct password for flag: dba8
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_cd6ed2eb}

```
para este fue a la fuerza y coloque cada una de las contrasenias hasta encontrar la correcta.
## Notas Adicionales

## Referencias