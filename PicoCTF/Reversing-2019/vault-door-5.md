# PicoCTF

## Descripcion
In the last challenge, you mastered octal (base 8), decimal (base 10), and hexadecimal (base 16) numbers, but this vault door uses a different change of base as well as URL encoding! The source code for this vault is here: [VaultDoor5.java](https://jupiter.challenges.picoctf.org/static/0a53bf0deaba6919f98d8550c35aa253/VaultDoor5.java)

## Pistas
1. You may find an encoder/decoder tool helpful, such as https://encoding.tools/
2.  Read the wikipedia articles on URL encoding and base 64 encoding to understand how they work and what the results look like.
## Solucion 
Vamos a cyberchef, colocamos el texto que esta codificado en url, y en base 64 y tenemos la bandera.
picoCTF{c0nv3rt1ng_fr0m_ba5e_64_0b957c4f}

## Notas Adicionales

## Referencias