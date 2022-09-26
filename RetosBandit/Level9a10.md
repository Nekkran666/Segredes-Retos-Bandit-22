# Level9a10

## Objetivo
The password for the next level is stored in the file **data.txt** in one of the few human-readable strings, preceded by several ‘=’ characters.

## Datos de acceso
bandit9
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

## Solucion

```
bandit9@bandit:~$ cat data.txt | string | grep ==
========== the*2i*4
========== password
Z)========== is
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
```
truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

## Notas adicionales
Para encontrar cadenas onlly human readable la cual tenga determinados caracteres le pasamos cat "string" para filtrar solo a cadenas "grep".

## Referencias

