# Level 7 a 8

## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**

## Datos de acceso
bandit7
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

## Solucion
```
bandit7@bandit:~$ cat data.txt | grep millionth
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
bandit7@bandit:~$
```
cvX2JJa4CFALtqS87jk27qwqGhBM9plV

## Notas adicionales

Para escapar de la salida de un comando con otro comando se usan "|" en este caso la salida de cat pasa al comando grep filtrando solo la linea que contenga "millionth"

## Referencias

