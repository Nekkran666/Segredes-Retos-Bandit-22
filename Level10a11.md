# Level10a11

## Objetivo
The password for the next level is stored in the file **data.txt**, which contains base64 encoded data

## Datos de acceso
bandit10
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

## Solucion
```
bandit10@bandit:~$ cat data.txt | base64 -d
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
bandit10@bandit:~$
```
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Notas adicionales

## Referencias
https://en.wikipedia.org/wiki/Base64
