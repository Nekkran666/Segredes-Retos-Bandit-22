# Level6a7

## Objetivo
The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

## Datos de acceso
bandit6
DXjZPULLxYr17uwoI01bNLQbtFemEgo7

## Solucion
```
bandit6@bandit:~$ find / -readable -user bandit7 -group bandit6 -size 33c
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## Notas adicionales
Para encontrar algun archivo de algun usuario, de un cierto tamanio, debemos utilizar find con unos parametros en especificos, los ciales son -user -group, size.

## Referencias