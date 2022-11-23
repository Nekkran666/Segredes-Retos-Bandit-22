# unpackme.py

## Descripcion
Can you get the flag? Reverse engineer this [Python program](https://artifacts.picoctf.net/c/465/unpackme.flag.py).

## Pistas

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/reversing22/up]
└─$ open unpackme.flag.py                  
                                                                                                 
┌──(kali㉿kali)-[~/PicoCTF/reversing22/up]
└─$ python3 unpackme.flag.py            

pw = input('What\'s the password? ')

if pw == 'batteryhorse':
  print('picoCTF{175_chr157m45_cd82f94c}')
else:
  print('That password is incorrect.')


```
en ver de hacer que ejecute la linea 12, hacemos que la imprima.
## Notas Adicionales

## Referencias