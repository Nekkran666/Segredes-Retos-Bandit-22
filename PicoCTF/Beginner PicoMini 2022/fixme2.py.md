# fixme2.py

## Descripcion
Fix the syntax error in the Python script to print the flag.

## Pistas
1. Are equality and assignment the same symbol?
2. To view the file in the webshell, do: `$ nano fixme2.py`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.

## Solucion 
```bash
──(kali㉿kali)-[~/Downloads]
└─$ python3 fixme2.py
  File "/home/kali/Downloads/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme2.py   
                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme2.py
                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_f6a5aefc}

```
agregue un = al if


## Notas Adicionales

## Referencias