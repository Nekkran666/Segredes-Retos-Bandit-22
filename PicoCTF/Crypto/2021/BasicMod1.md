# basic-mod1

## Descripcion
We found this weird message being passed around on the servers, we think we have a working decryption scheme. Download the message [here](https://artifacts.picoctf.net/c/395/message.txt). Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore. Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)

## Pistas
1. Do you know what `mod 37` means?
2. `mod 37` means modulo 37. It gives the remainder of a number after being divided by 37.

## Solucion
```bash
datos = open('message.txt').read().split()

print(datos)

flag = ''

for n in datos:
        c = int(n) % 37
        if c >= 0 and c <= 25:
                s = chr(c + 65)
        elif c >= 26 and c <= 35:
                s = chr(c+22)
        else:
                s = '_'
        flag += s

print (f"picoCTF{{{flag}}}")

┌──(kali㉿kali)-[~/PicoCTF/crypto22/mod1]
└─$ python3 exp.py
['91', '322', '57', '124', '40', '406', '272', '147', '239', '285', '353', '272', '77', '110', '296', '262', '299', '323', '255', '337', '150', '102']
picoCTF{R0UND_N_R0UND_ADD17EC2}
                                

```


## Notas Adicionales

## Referencias