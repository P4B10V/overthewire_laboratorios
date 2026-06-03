**Nivel 1 -> 2**

[Enunciado original](https://overthewire.org/wargames/krypton/krypton1.html)

**Descripción**

The password for level 2 is in the file ‘krypton2’. It is ‘encrypted’ using a simple rotation. It is also in non-standard ciphertext format. When using alpha characters for cipher text it is normal to group the letters into 5 letter clusters, regardless of word boundaries. This helps obfuscate any patterns. This file has kept the plain text word boundaries and carried them to the cipher text. Enjoy!

**Solución**

Si ya pasamos antes por el [wargame Bandit](https://overthewire.org/wargames/bandit/) ya deberíamos de conocer el uso del comando `base64`, con esto ya es suficiente para resolver este nivel. 

Por estudiar un poco en el tema, base64 es una técnica que nos permite codificar información (transformar de un formato a otro) de manera que podamos revertir su codificación. 

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
