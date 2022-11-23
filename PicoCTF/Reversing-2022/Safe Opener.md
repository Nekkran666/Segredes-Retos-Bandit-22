# Safe Opener

## Descripcion
Can you open this safe? I forgot the key to my safe but this [program](https://artifacts.picoctf.net/c/463/SafeOpener.java) is supposed to help me with retrieving the lost key. Can you help me unlock my safe? Put the password you recover into the picoCTF flag format like: `picoCTF{password}`

## Pistas

## Solucion 
```bash 
┌──(kali㉿kali)-[~/PicoCTF/reversing22/sop]
└─$ nano SafeOpener.java 
                                                                                                 
┌──(kali㉿kali)-[~/PicoCTF/reversing22/sop]
└─$ echo cGwzYXMzX2wzdF9tM18xbnQwX3RoM19zYWYz | base64 -d
pl3as3_l3t_m3_1nt0_th3_saf3   
```
Hacemos un nano al programa que descargamos buscamos el string encode, lo pasamos a base64 y listo tenemos la bandera.
## Notas Adicionales

## Referencias