# fixme1.py

## Descripcion
Fix the syntax error in this Python script to print the flag.
## Pistas
1. Indentation is very meaningful in Python
2. To view the file in the webshell, do: `$ nano fixme1.py`
3. To exit `nano`, press Ctrl and x and follow the on-screen prompts.
4. The `str_xor` function does not need to be reverse engineered for this challenge.

## Solucion 
```bash
──(kali㉿kali)-[~/Downloads]
└─$ python3 fixme1.py
  File "/home/kali/Downloads/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme1.py   
                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ python3 fixme1.py
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_09ee727a}

```
## Notas Adicionales

## Referencias