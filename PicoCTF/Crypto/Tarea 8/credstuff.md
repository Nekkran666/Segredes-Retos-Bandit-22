# credstuff

## Descripcion
We found a leak of a blackmarket website's login credentials. Can you find the password of the user `cultiris` and successfully decrypt it? Download the leak [here](https://artifacts.picoctf.net/c/534/leak.tar). The first user in `usernames.txt` corresponds to the first password in `passwords.txt`. The second user corresponds to the second password, and so on.

## Pistas
1. Maybe other passwords will have hints about the leak?

## Solucion 
Descargamos el archivo que nos dan en pico, descomprimimos, buscamos el usuario que nos dan, se encuentra en la lina 378, en los passwords buscamos la misma linea, y nos damos cuenta que tiene unas llaves, despues lo pasamos a un decodificador caesar y obtenemos la bandera.
picoCTF{C7r1F_54V35_71M3}

## Notas Adicionales

## Referencias