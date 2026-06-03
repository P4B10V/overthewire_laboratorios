**Nivel 31 → 32**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit32.html)

**Descripción**

El procedimiento es prácticamente el mismo que en el nivel anterior. Debemos acceder al repositorio Git mediante: `ssh://bandit31-git@bandit.labs.overthewire.org/home/bandit31-git/repo` utilizando el puerto **2220**.  

La contraseña es la misma que la del usuario **bandit31**.

**Solución**

Este nivel ya me gustó bastante más. Después de clonar el repositorio localmente e investigar encontré:

```
+This time your task is to push a file to the remote repository.
+
+Details:
+    File name: key.txt
+    Content: 'May I come in?'
+    Branch: master
```

Así que mi suposición sería crear el archivo dentro del repositorio, llamarlo igual con el mismo contenido y subirlo al repositorio. 

El objetivo es `subir al archivo al repositorio`, si este paso se hace correctamente se obtiene la contraseña del siguiente nivel.

**Comandos sugeridos**

`git`

**Contenido sugerido**

- *Installing Git*  
- *Git from the Bottom Up*

*Las credenciales y soluciones exactas no serán escritas. Aunque se trate de un juego, este documento se centra únicamente en los pasos, razonamientos y errores cometidos durante la resolución.*
