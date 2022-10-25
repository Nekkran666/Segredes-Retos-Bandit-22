# Wireshark doo dooo do doo...

## Descripcion
Can you find the flag? [shark1.pcapng](https://mercury.picoctf.net/static/d6f9aa16d2a2c51d2e431e658d87af9e/shark1.pcapng).

## Pistas

## Solucion 
Descargamos el archivo de paquetes que nos entrega el reto, y comenzamos a observarlo en wireshark, observamos que hay muchos paquetes encriptados, y hay un http que no esta encriptado, lo seguimos y observamos algo parecido enuna llave que se encuentra en rot13, la pasamos a texto plano y tenemos la bandera.
picoCTF{p33kab00_1_s33_u_deadbeef}

## Notas Adicionales

## Referencias