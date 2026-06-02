**Nivel 22 -> 23**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit23.html)

**Descripción**

Un programa está corriendo a intervalos regulares desde cron. Mira en `/etc/cron.d/`para ver la configuración y ver que comando se está ejecutando.

**Solución**

Para la resolución de este nivel tendremos que estudiar el siguiente script:

```bash
#!/bin/bash
myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"
cat /etc/bandit_pass/$myname > /tmp/$mytarget
```

Si nos damos cuenta, podemos ver que hay dos ubicaciones que tiene la contraseña, una es: /etc/bandit_pass/bandit23 y la otra /tmp/$mytarget. 
Al intentar la primera, nos dará permiso denegado, por lo que tendremos que comprobar si podemos en /tmp 

¿Hay alguna manera de descubrir el nombre? Si leemos otra vez el script, podemos ver que $mytarget es el nombre del archivo, y se genera en ese script, por lo que si ejecutamos:

echo I am user $myname | md5sum | cut -d ' ' -f 1 ya tendriamos la ruta, presta atención a quien es $myname

*Comandos sugeridos*
`cron`, `crontab`, `crontab(5) (use “man 5 crontab” to access this)`



*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
