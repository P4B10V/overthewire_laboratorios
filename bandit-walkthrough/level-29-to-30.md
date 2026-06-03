**Nivel 30 → 31**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit29.html)

**Descripción**

El procedimiento es prácticamente el mismo que en el nivel anterior. Debemos acceder al repositorio Git mediante: `ssh://bandit28-git@bandit.labs.overthewire.org/home/bandit29-git/repo` utilizando el puerto **2220**.  

La contraseña es la misma que la del usuario **bandit29**.

**Solución**

Tras clonar el repositorio, comencé revisando el historial con comandos como `git log` y `git show`, pero no encontraba nada relevante. Finalmente, al cambiar de *branch*, apareció la información necesaria.  
Este nivel, igual que los anteriores, se basa en experimentar: probar comandos, revisar qué devuelve cada uno y explorar las ramas disponibles.

No presenta gran dificultad técnica; simplemente requiere paciencia, curiosidad y revisar bien las opciones que ofrece `git`.

**Comandos sugeridos**

- `git`

**Contenido sugerido**

- *Installing Git*  
- *Git from the Bottom Up*

*Las credenciales y soluciones exactas no serán escritas. Aunque se trate de un juego, este documento se centra únicamente en los pasos, razonamientos y errores cometidos durante la resolución.*

