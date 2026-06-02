**Nivel 18 -> 19**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit19.html)

**Descripción**

La contraseña esta almacenada en el fichero `readme` ubicado en el home del usuario. Por desgracia, alguien modifico .bashrc para desconectarte cuando te logeas por ssh.

**Solución**

Para resolver este nivel, tendremos que aprender una función de `ssh` y es que nos permite ejecutar comandos remotamente en la máquina en la que realizamos la conexión. Es decir, que si al conectarnos tratamos de leer el contenido del fichero, aunque nos eche podremos obtenerlo igualmente.


*Comandos sugeridos*

`ssh`, `ls`, `cat`



*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
