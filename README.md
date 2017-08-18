Muchas veces al utilizar la libreria PyVirtualDisplay en Python, se ejecuta Xvfb en segundo plano y no se cierra al 
terminar la ejecución provocando la utilización de recursos innecesarios en el servidor.

La ejecución de estos comandos te permitiran cerrar todos los procesos Xvfb:   
ps aux | grep Xvfb | awk '{print "kill", $2}' | sh  2>/dev/null
