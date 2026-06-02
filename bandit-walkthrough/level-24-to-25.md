**Nivel 24 -> 25**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit25.html)

**Descripción**

Un demonio está escuchando en el puerto 30002 y te dará la contraseña de bandit25 si le das la contraseña de bandit24 y un pin de 4 digitos correctos. Necesitaremos usar fuerza bruta para hacer las 10000 combinaciones, y no hace falta hacer una conexión cada vez.

**Solución**

Lo primero que se me ocurrio fue realizar una simple conexión a ese puerto (antes comprobé si existía un servicio escuchando con `nmap`) y conseguimos una respuesta:

```
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
```

Ahora que sabemos que el formato será [CONTRASEÑA] [PIN] deberemos de idear una manera de iterar todo ese rango de numeros.

Lo que se me ocurrió fue crear un bucle for que iterara desde el 0000 hasta el 9999 y a cada iteracción realizara la conexión, como no fui capaz de filtrar bien los datos lo que hice fue mandar ese resultado a un documento de texto y mediante `grep` consegui la contraseña de bandit25.

Como añadido, existe un *parámetro* de nc que corta la conexión una vez que termina.


*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
