**Nivel 23 -> 24**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit24.html)

**Descripción**

Un programa está corriendo a intervalos regulares desde cron. Mira en `/etc/cron.d/`para ver la configuración y ver que comando se está ejecutando.
NOTAS: Este nivel requiere crear un script. El script se borrará por lo que si lo quieres mantener guardalo porque no lo podrás recuperar.

**Solución**

Nuestro objetivo es conseguir la contraseña de `bandit24` por lo que buscaremos la tarea programada con ese nombre, una vez encontrado tendremos que analizar el script para ver que hace.

Lo que mas me llamó la atención del script fue `echo "Executing and deleting all scripts in /var/spool/$myname/foo:"` es decir:
Si fueramos capaces de poner un script ahi se ejecutaría como dicho usuario.

El problema que me encontré fue que al poner el script no ocurría nada, al final el problema se basaba en `permisos`

Para no ensuciar el entorno utilicé `mktemp -d` para crear un directorio temporal y modificar sus permisos, una vez que todo el mundo podía escribir ahi, la contraseña apareció.

*Comandos sugeridos*
`cron`, `crontab`, `crontab(5) (use “man 5 crontab” to access this)`



*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
