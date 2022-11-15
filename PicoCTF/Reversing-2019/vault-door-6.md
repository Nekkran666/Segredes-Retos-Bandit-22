# valut-door-6

## Descripcion
This vault uses an XOR encryption scheme. The source code for this vault is here: [VaultDoor6.java](https://jupiter.challenges.picoctf.org/static/cdb33ffba609e2521797aac66320ec65/VaultDoor6.java)

## Pistas
1. If X ^ Y = Z, then Z ^ Y = X. Write a program that decrypts the flag based on this fact.

## Solucion 
```bash
>>> mybytes = [0x3b, 0x65, 0x21, 0xa , 0x38, 0x0 , 0x36, 0x1d, 0xa , 0x3d, 0x61, 0x27, 0x11, 0x66, 0x27, 0xa , 0x21, 0x1d, 0x61, 0x3b, 0xa , 0x2d, 0x65, 0x27, 0xa , 0x6c, 0x60, 0x37, 0x30, 0x60, 0x31, 0x36,]
>>> mybytes
[59, 101, 33, 10, 56, 0, 54, 29, 10, 61, 97, 39, 17, 102, 39, 10, 33, 29, 97, 59, 10, 45, 101, 39, 10, 108, 96, 55, 48, 96, 49, 54]
>>> flag = [ i ^ 0x55 for i in mybytes ]
>>> flag
[110, 48, 116, 95, 109, 85, 99, 72, 95, 104, 52, 114, 68, 51, 114, 95, 116, 72, 52, 110, 95, 120, 48, 114, 95, 57, 53, 98, 101, 53, 100, 99]
>>> flag = [ chr(i) for i in flag ]
>>> flag
['n', '0', 't', '_', 'm', 'U', 'c', 'H', '_', 'h', '4', 'r', 'D', '3', 'r', '_', 't', 'H', '4', 'n', '_', 'x', '0', 'r', '_', '9', '5', 'b', 'e', '5', 'd', 'c']
>>> ''.join(flag)
'n0t_mUcH_h4rD3r_tH4n_x0r_95be5dc'
>>> 
```
picoCTF{n0t_mUcH_h4rD3r_tH4n_x0r_95be5dc}

## Notas Adicionales

## Referencias