# Level 2 a 3

## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory

## Datos de acceso
bandit2
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

## Solucion
```
bandit2@bandit:~$ ls
spaces in this filename
bandit2@bandit:~$ cat spaces\ in\ this\ filename
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
bandit2@bandit:~$
```


UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Notas adicionales
Tenemos que utilizar \ para eliminar los espacios que hay en el nombre del archivo para asi poder ver su contenido.

## Referencias