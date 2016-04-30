Ejercicios Tema 5  
=================  

T5.1  
----  
**Buscar información sobre cómo calcular el número de conexiones por segundo.**  

1)Si tenemos un servidor Apache:
el comando apache2ctl status muestra el número de peticiones que está cursando el servidor:

*apache2ctl status |grep request*

Si queremos más información de las conexiones existe el paquete iptstate. 

Ipstate permite de filtrar la salida del comando para que te diga el número de conexiones a un puerto determinado de una dirección IP, por ejemplo:

*iptstate -1 -d 192.168.0.100 -D 80*

Lo bueno de iptstate es que se puede controlar el número de conexiones a uno o varios servidores apache (o de otros servicios) desde fuera de los propios servidores si se ejecuta en el firewall.

2)IPTraf es una utilidad de monitorización de código abierto basada en consola y en tiempo real de la red para Linux. (IP LAN) - Recoge una gran variedad de información como monitor de tráfico IP que pasa a través de la red, incluida la información de flags TCP, detalles ICMP, TCP / averías tráfico UDP, paquete de conexión TCP y cuenta Byne. También recoge información de estadísticas de la interfaz general y detaled de TCP, UDP, errores de suma de comprobación IP no IP ICMP IP, interfaz actividad, etc



T5.3  
----  
**Buscar información sobre características, disponibilidad para diversos SO, etc de herramientas para monitorizar las prestaciones de un servidor. Para empezar, podemos comenzar utilizando las clásicas de Linux: top, vmstat, netstat**  

El Comando **Top** Linux es un programa para la supervisión del rendimiento que utilizan con mucha frecuencia la mayoría de los administradores de sistemas para comprobar el rendimiento de Linux y está disponible en muchos sistemas Linux / Unix. El comando top se utiliza para mostrar todo el funcionamiento y los procesos en tiempo realmente activos en una lista que actualiza regularmente. Se mostrará el uso de CPU, uso de memoria, la memoria de intercambio, Cache, Tamaño de búfer, PID de proceso, usuario, Comandos y mucho más. También muestra la carga de memoria y de la CPU de un proceso en ejecución. El comando top es mucho útil para el administrador de sistema para supervisar y tomar acción correcta cuando se requiera. 

Comando **vmstat** de Linux se utiliza para mostrar las estadísticas de la memoria virtual, hilos kernerl, discos, procesos de sistema, bloques de E / S, interrupciones, actividad de la CPU y mucho más. Al comando vmstat predeterminada no está disponible en los sistemas Linux es necesario instalar un paquete llamado sysstat que incluye un programa vmstat. 

Comando **lsof** se utiliza en muchos Linux / Unix como sistema que se utiliza para motar todos los archivos abiertos y los procesos que los utilizan. Los archivos abiertos incluidos son archivos de disco, de la red, tuberías, dispositivos y procesos. Una de las principales razones para el uso de este comando es que cuando un disco no se puede desmontar y muestra el error de que hay archivos que lo están utilizando o están. Con este comando puede identificar fácilmente qué archivos están en uso.

**Tcpdump** es el analizador de paquetes de la línea de comandos más utilizado o programa de succionador de paquetes que se utiliza tanto para la captura o el filtro de paquetes TCP/IP que recibieron o han sido transferidos en una interfaz específica a través de una red. También proporciona una opción para guardar los paquetes capturados en un archivo para su posterior análisis. tcpdump esta casi siempre disponible en las principales distribuciones de Linux.

**Netstat** es una herramienta de línea de comandos para controlar los paquetes de red, estadísticas entrantes y salientes, así como estadísticas de la interfaz. Es una herramienta muy útil para todos los administradores de sistema para monitorear el desempeño de la red y solucionar problemas relacionados con la red.