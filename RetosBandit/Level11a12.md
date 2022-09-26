# Level11a12

## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Datos de acceso
bandit11
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Solucion
```
bandit11@bandit:~$ cat data.txt | tr 'n-za-mN-ZA-M' 'a-zA-Z'
The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
bandit11@bandit:~$
```
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Notas adicionales
Se utiliza el cat para leer el archivo y tr para descencriptarlo, ya que tr es un comando de linux utilizado para traducir o borrar de un input y escribir el resultado en un output.

## Referencias

