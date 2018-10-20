---
title: 10 Simple and Useful Linux Commands
localeTitle: 10 comandos de Linux simples y útiles
---
# 10 comandos de Linux simples y útiles

Los comandos que se enumeran aquí son básicos y te ayudarán a comenzar rápidamente. Sin embargo, son también poderosos, y seguirán siendo útiles a medida que se expanda tu experiencia en Linux.

1.  `echo` Este comando toma el texto que le das y lo envía de regreso a algún lugar como la pantalla, a un archivo u a otro comando. Ejemplo: `echo "hello!"`
2.  `cat` Para mostrar el contenido de un archivo de texto, simplemente escribe `cat myfile` .
3.  `find` hace lo que dice (buscar), y es bueno en eso. Úsalo para localizar archivos por ruta (path), tamaño, fecha, propietario y un montón de otros filtros útiles. Ejemplo: `find . -type f -mtime -1h # List files in this directory modified in the past hour` .
4.  `date` Simplemente escribe date (fecha) cuando desees saber qué hora es. Ejemplo: `date "+It's %l:%m%p on %A"` . Úsalo en un script para nombrar archivos de acuerdo con la fecha actual.
5.  `ls` ¿Qué hay en este directorio? Combina `ls` con algunas marcas (flags) útiles para mostrar y ordenar los contenidos del directorio por fecha y tamaño. También te da muchas opciones para formatear el resultado.
6.  `pwd` ¿Dónde estoy? Linux puede ser implacable, especialmente cuando borras algo. Asegúrate de que sabes dónde estás antes de emitir tus comandos.
7.  `mail` El programa de correo de Linux no es atractivo, pero puede ser realmente útil. Puedes crear un mensaje y agregar texto, destinatarios y archivos adjuntos en un sólo comando. Ejemplo: `echo "We're having a great time." | mail -s "Wish you were here!" -A postcard.png -t mom@example.com`
8.  `cut` Cuando tenga una cadena con separadores, usa `cut` para filtrar ciertos campos. Ejemplo: `echo "this, that, and the other" | cut -d, -f2 # "that"`
9.  `grep` Para encontrar líneas de texto que contengan una determinada cadena, usa grep. Ejemplo: `grep 'root' /etc/passwd # root:x:0:0:root:/root:/bin/bash`
10.  `sed` Utilice sed para buscar y cambiar una subcadena en un texto. Ejemplo: `echo "this, that, and the other" | sed 's/that/those/' # "this, those, and the other"`
11.  `shutdown` Úsalo para apagar el sistema y la alimentación. Ejemplo: `shutdown -h now` apaga el sistema inmediatamente. `shutdown -h +5` apaga el sistema después de cinco minutos.

Utiliza estos comandos en scripts y en la línea de comandos. Todos son comandos muy poderosos, y la página del manual de Linux tiene mucha más información sobre cada uno.

* * *

Además, los comandos importantes utilizados para los administradores del sistema son los siguientes:

1. `uptime` El comando uptime en Linux muestra cuánto tiempo se ha estado ejecutando tu sistema y la cantidad de usuarios que han iniciado sesión. También muestra el promedio de carga en intervalos de 1,5 y 15 minutos.
    
2.  `w` Este comandp mostrará los usuarios que han iniciado sesión y su proceso junto con los promedios de carga. también muestra el nombre de inicio de sesión, nombre de tty, host remoto, tiempo de inicio de sesión, tiempo de inactividad, JCPU, PCPU, comandos y procesos.
    
3.  `users` El comando de usuarios muestra usuarios actualmente conectados. Este comando no tiene otros parámetros aparte de la ayuda y la versión.
    
4.  `who` El comando quién simplemente devuelve el nombre de usuario, la fecha, la hora y la información del host. who command es similar a w command, la diferencia es que el comando who no imprime lo que hacen los usuarios. Illustremos los diferentes comandos de who y w.
    
5.  Comando `whoami` El comando whoami imprime el nombre del usuario actual. También puedes usar el comando "quién soy yo" para mostrar el usuario actual. Si ha iniciado sesión como root, utilice el comando sudo "whoami" y regresa a root como usuario actual. Usa el comando "quién soy yo" si desea conocer el usuario exacto que inició sesión.
    
6.  `ls` El comando ls muestra la lista de archivos en formato legible por humanos.
    
7.  `crontab` Este comando crea una lista de trabajos de programación para el usuario actual con el comando crontab y la opción -l.
    
8.  `less` Comando menos permite ver rápidamente el archivo. Puedes subir y bajar la página. Presiona 'q' para salir de la ventana del comando less.
    
9.  `more` Comando más te permite ver rápidamente el archivo mostrando los detalles en porcentaje. Puedes subir y bajar la página. Presiona 'q' para salir de la ventana del comando more.
    
10.  Comando `cp` copia el archivo desde el origen al destino conservando el mismo modo.
    

Aquí está la lista de comandos utilizados con frecuencia por un administrador. Esto no es una lista completa, pero es compacta para consultar cuando sea necesario.
