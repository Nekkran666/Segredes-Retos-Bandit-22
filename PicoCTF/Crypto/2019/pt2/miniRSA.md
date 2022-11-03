# miniRSA

## Descripcion
Let's decrypt this: [ciphertext](https://jupiter.challenges.picoctf.org/static/d21037ad23ed84cfff20a84768a0f2b2/ciphertext)? Something seems a bit small.

## Pistas
1. RSA [tutorial](https://en.wikipedia.org/wiki/RSA_(cryptosystem))
2. How could having too small an e affect the security of this 2048 bit key?
3. Make sure you don't lose precision, the numbers are pretty big (besides the e value)

## Solucion 
Para este reto, descargamos un archivo de pico, donde se encuentra un texto cifrado den RSA, nos damos cuenta que la la e que nos entregan es muy corta, por lo cual la seguridad es muy baja, utilizando un corto codigo en python se consiguio la llave
```bash
>>> gmpy2.get_context().precision+2048
2101
>>> e = 3
>>> c = 2205316413931134031074603746928247799030155221252519872650073010782049179856976080512716237308882294226369300412719995904064931819531456392957957122459640736424089744772221933500860936331459280832211445548332429338572369823704784625368933
>>> 
>>> root, exact = iroot(c, e)
>>> root
mpz(13016382529449106065894479374027604750406953699090365388203708028670029596145277)
>>> print( long_to_bytes(root) )
b'picoCTF{n33d_a_lArg3r_e_ccaa7776}'
>>> 

```

picoCTF{n33d_a_lArg3r_e_ccaa7776}

## Notas Adicionales

## Referencias