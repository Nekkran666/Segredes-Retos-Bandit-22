# MiniRSA

## Descripcion
What happens if you have a small exponent? There is a twist though, we padded the plaintext so that (M ** e) is just barely larger than N. Let's decrypt this: [ciphertext](https://mercury.picoctf.net/static/2d884b04dbb44896dda1276774b09216/ciphertext)

## Pistas
1. RSA [tutorial](https://en.wikipedia.org/wiki/RSA_(cryptosystem))
2. How could having too small of an `e` affect the security of this key?
3. Make sure you don't lose precision, the numbers are pretty big (besides the `e` value)
4. You shouldn't have to make _too_ many guesses
5. `pico` is in the flag, but not at the beginning

## Solucion 

## Notas Adicionales

## Referencias