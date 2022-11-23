# buffer overflow 0

## Descripcion
Smash the stack Let's start off simple, can you overflow the correct buffer? The program is available [here](https://artifacts.picoctf.net/c/521/vuln). You can view source [here](https://artifacts.picoctf.net/c/521/vuln.c). And connect with it using: `nc saturn.picoctf.net 65355`

## Pistas
1.  How can you trigger the flag to print?
2. If you try to do the math by hand, maybe try and add a few more characters. Sometimes there are things you aren't expecting.
3. Run `man gets` and read the BUGS section. How many characters can the program really read?

## Solucion 

## Notas Adicionales

## Referencias