# file-run2

## Descripcion
Another program, but this time, it seems to want some input. What happens if you try to run it on the command line with input "Hello!"? Download the program [here](https://artifacts.picoctf.net/c/352/run).

## Pistas
1. Try running it and add the phrase "Hello!" with a space in front (i.e. "./run Hello!")

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr2]
└─$ chmod +x run           
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr2]
└─$ ./run           
Run this file with only one argument.
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr2]
└─$ ./run hello 
Won't you say 'Hello!' to me first?
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr2]
└─$ ./run Hello!
The flag is: picoCTF{F1r57_4rgum3n7_96f2195f}   
```


## Notas Adicionales

## Referencias