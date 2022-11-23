# file-run1

## Descripcion
A program has been provided to you, what happens if you try to run it on the command line? Download the program [here](https://artifacts.picoctf.net/c/309/run)

## Pistas
1. To run the program at all, you must make it executable (i.e. `$ chmod +x run`)
2. Try running it by adding a '.' in front of the path to the file (i.e. `$ ./run`)

## Solucion 
```bash
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr1]
└─$ python3 run   
SyntaxError: Non-UTF-8 code starting with '\xff' in file /home/kali/PicoCTF/reversing22/fr1/run on line 2, but no encoding declared; see https://python.org/dev/peps/pep-0263/ for details
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr1]
└─$ ./run           
zsh: permission denied: ./run
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr1]
└─$ chmod +x run           
                                                                                                
┌──(kali㉿kali)-[~/PicoCTF/reversing22/fr1]
└─$ ./run       
The flag is: picoCTF{U51N6_Y0Ur_F1r57_F113_e5559d46
```

## Notas Adicionales

## Referencias