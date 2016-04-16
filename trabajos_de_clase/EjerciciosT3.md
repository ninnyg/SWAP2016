##Ejercicios Tema 3

#T3.1
**Buscar con qué órdenes de terminal o herramientas gráficas podemos configurar bajo Windows y bajo Linux el enrutamiento del tráfico de un servidor para pasar el tráfico desde una subred a otra.**

*Linux*

Command : route add -net 192.168.3.0 netmask 255.255.255.0 gw 192.168.3.10

![imagen](https://github.com/ninnyg/SWAP2016/blob/master/trabajos_de_clase/route.png)

Now all the packets addressed to 192.168.3.* network will be forwarded via the 192.168.3.10 interface, which then delivers the packets to the addressed machine.

Source:  http://www.thegeekstuff.com/2012/04/route-examples/


*Windows*

Command : route add 1.1.1.0 mask 255.255.255.0 10.0.1.1 if 1

Source: http://www.windowsnetworking.com/articles-tutorials/network-protocols/How-configure-Windows-2008-Server-IP-Routing.html


#T3.2
**Buscar con qué órdenes de terminal o herramientas gráficas podemos configurar bajo Windows y bajo Linux el filtrado y bloqueo de paquetes.**

*Linux*
La principal orden en Linux es iptables, que nos permite incluir múltiples reglas para dejar pasar o bloquear paquetes, siendo una herramienta ampliamente conocida.

Es. iptables -A INPUT -s 127.0.0.1 -p icmp -j DROP

Source: http://www.netfilter.org/documentation/HOWTO/es/packet-filtering-HOWTO-7.html


*Windows*
En Windows, se puede agregar un filtrado de paquetes mediante la herramienta de Enrutamiento y acceso remoto.

Source: 
https://msdn.microsoft.com/es-es/library/cc738952(v=ws.10).aspx

Source: 
https://technet.microsoft.com/es-es/library/cc732746(v=ws.10).aspx