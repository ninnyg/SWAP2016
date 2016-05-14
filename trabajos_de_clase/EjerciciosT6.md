#Ejercicio T6.1: Aplicar con iptables una política de denegar todo el tráfico en una de las máquinas de prácticas. Comprobar el funcionamiento.

En las imagenes se muestra cómo al añadir la regla de no aceptar ningún tipo de tráfico no se descarga la página /index.html.
Luego se ha eliminado esta regla y se ha incluido la política de permitir todo el tráfico. Entonces sí se puede acceder a la página en cuestión. 

![imagen](https://github.com/ninnyg/SWAP2016/blob/master/trabajos_de_clase/iptables.png)
![imagen](https://github.com/ninnyg/SWAP2016/blob/master/trabajos_de_clase/iptables2.png)


#Ejercicio T6.3:  Buscar información acerca de los tipos de ataques más comunes en servidores web, en qué consisten, y cómo se pueden evitar.

##SQL Injection - La inyección de código SQL puede usarse para ganar acceso al área privada de una Web, robar o borrar información, hacer modificaciones en la Web, o incluso, tomar el control total del servidor con todas las bases de datos y Webs que existan en éste. Habitualmente, estos ataques se llevan a cabo haciendo uso de la comilla simple, que cierra una cadena en SQL y de “- -” que se utiliza para poner comentarios.
La forma de prevenir estos ataques es utilizar, como mínimo, las funciones de filtrado que nos proporcionan los distintos frameworks de desarrollo y, procurar siempre establecer la codificación de la página ya que si acepta varias codificaciones, pueden saltarse el filtro introduciendo caracteres en UTF7.
Se puede evitar poniendo atención en los lugares donde el usuario nos pasa información, comprobando que no puede realizar de ningún modo una consulta. 

##La Denegación de Servicio (DoS) ó Denegación de Servicio Distribuida (DDoS) son las formas más comunes para congelar el funcionamiento de un sitio web. Estos son los intentos de inundar un sitio con solicitudes externas, por lo que ese sitio no podría estar disponible para los usuarios reales. Los ataques de denegación de servicio por lo general se dirigen a puertos específicos, rangos de IP o redes completas, pero se pueden dirigir a cualquier dispositivo o servicio conectado.
Los ataques de denegación de servicio funcionan cuando una computadora con una conexión a Internet intenta inundar un servidor con paquetes. DDoS, por otro lado son cuando muchos dispositivos, a menudo ampliamente distribuidos, en un intento de botnet para inundar el objetivo con cientos, a menudo miles de peticiones.

Los ataques DDoS vienen en 3 variedades principales:

Los ataques de volumen, donde el ataque intenta desbordar el ancho de banda en un sitio específico.
Los ataques de protocolo, donde los paquetes intentan consumir servicios o recursos de la red.
Ataques a aplicaciones, donde las peticiones se hacen con la intención de “explotar” el servidor web, mediante la capa de aplicación.

La solución a esto consiste en disponer de cortafuegos o un buen sistema de seguridad que identifique rápidamente si se trata de un ataque de denegación de servicio y repeler a la máquina o máquinas que lo estén realizando.