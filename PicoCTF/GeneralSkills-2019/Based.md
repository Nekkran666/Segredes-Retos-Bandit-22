# Based

## Descripcion
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with `nc jupiter.challenges.picoctf.org 29221`.

## Pistas
1. It might help to have multiple windows open.
2. I hear python can convert things.

## Solucion 
```bash
┌──(kali㉿kali)-[~/Downloads]
└─$ nc jupiter.challenges.picoctf.org 29221
Let us see how data is stored
submarine
Please give the 01110011 01110101 01100010 01101101 01100001 01110010 01101001 01101110 01100101 as a word.
...
you have 45 seconds.....

Input:
submarine
Please give me the  143 157 155 160 165 164 145 162 as a word.
Input:
^C
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ nc jupiter.challenges.picoctf.org 29221
Let us see how data is stored
pear
Please give the 01110000 01100101 01100001 01110010 as a word.
...
you have 45 seconds.....

Input:
pear
Please give me the  154 141 155 160 as a word.
Input:
Too slow!
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ nc jupiter.challenges.picoctf.org 29221
Let us see how data is stored
sludge
Please give the 01110011 01101100 01110101 01100100 01100111 01100101 as a word.
...
you have 45 seconds.....

Input:
sludge
Please give me the  163 157 143 153 145 164 as a word.
Input:
socket
Please give me the 636f6d7075746572 as a word.
Input:
computer
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_00a975ff}

```
![[Pasted image 20220924201257.png]]

![[Pasted image 20220924201326.png]]

![[Pasted image 20220924201341.png]]
## Notas Adicionales

## Referencias