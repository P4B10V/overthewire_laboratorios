**Nivel 19 -> 20**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit20.html)

**Descripción**

Para ganar acceso al siguiente nivel, deberás usar el binario ubicado en el directorio personal. Se puede ejecutar sin argumentos para saber cómo se usa. La contraseña puede ser encontrada en /etc/bandit_pass

**Solución**

Una vez dentro, ejecutamos el binario y nos dice `Run a command as another user` y como se llama bandit20-do podemos suponer que el usuario que lo ejecutará será bandit20. Pues bien, como las contraseñas ubicadas en `/etc/bandit_pass` sólo pueden ser leidas por el usuario correspondiente, usaremos `cat` pasándoselo como parametro y leyendo el archivo en la ruta que nos dieron. 

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
