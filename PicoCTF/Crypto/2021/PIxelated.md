# Pixelated

## Descripcion
I have these 2 images, can you make a flag out of them? [scrambled1.png](https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled1.png) [scrambled2.png](https://mercury.picoctf.net/static/6e4afb967ef8c865f79f3a8cd7767cca/scrambled2.png)

## Pistas
1. https://en.wikipedia.org/wiki/Visual_cryptography
2. Think of different ways you can "stack" images

## Solucion 
Se crea un script para cominar ambas imagenes.

```bash
from PIL import Image
import numpy as np
imagen1 = np.asarray(Image.open('scrambled1.png'))
imagen2 = np.asarray(Image.open('scrambled2.png'))

datos = imagen1.copy() + imagen2.copy()

nueva = Image.fromarray(datos)

nueva.save('nueva.png','PNG')

```

picoCTF{0542dc1d}

## Notas Adicionales

## Referencias