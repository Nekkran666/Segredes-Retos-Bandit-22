# vault-door-1

## Descripcion
This vault uses some complicated arrays! I hope you can make sense of it, special agent. The source code for this vault is here: [VaultDoor1.java](https://jupiter.challenges.picoctf.org/static/29b91e638ccbd76aaa8c0462d1c64d8d/VaultDoor1.java)

## Pistas
1. Look up the charAt() method online.

## Solucion 
creamos un nano donde colocamos los caracteres de password, y mediante consola y un cat, lo filtramos para que nos quedara la bandera,la pasamos al java y dice que es correcta.
```bash
┌──(kali㉿kali)-[~/PicoCTF/reversing19/door1]
└─$ cat bandera | sort | awk '{print($3)}' | tr -d "'" | tr -d "\n"
d35cr4mbl3_tH3_cH4r4cT3r5_ff63b0 
```
picoCTF{d35cr4mbl3_tH3_cH4r4cT3r5_ff63b0}

## Notas Adicionales

## Referencias