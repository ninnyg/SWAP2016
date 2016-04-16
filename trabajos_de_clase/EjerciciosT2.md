##Ejercicios Tema 2

#T2.1
**: Calcular la disponibilidad del sistema descrito en edgeblog.net si en cada subsistema tenemos en total 3 elementos**

| Components | Availability 1 el | Availability 2 el | Availability 3 el |
| :--------: |:-----------------:|:-----------------:|:-----------------:|
|  Web       | 85%               | 97.75%            | 99.66%  
| Application| 90%               | 99%               | 99.9%
| Database   | 99.9%             | 99.9999%          | 99.9999999%
| DNS        | 98%               | 99.96%            | 99.9992%
| Firewall   | 85%               | 97.75%            | 99.66%
| Switch     | 99%               | 99.99%            | 99.9999%
| Data Center| 99.99%            | 99.99%            | 99.99%
| ISP        | 95%               | 99.75%            | 99.9875%
| TOTAL      | 59.87%            | 94.30%            | 99.19%



#T2.2
**Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad**

*NodeJS*
•PM2 - PM2 is a production process manager for Node.js applications with a built-in load balancer. It allows you to keep applications alive forever, to reload them without downtime and will facilitate common system admin tasks. It also enables you to manage application logging, monitoring, and clustering.
•StrongLoop - StrongLoop Process Manager (StrongLoop PM) is a production process manager for Node.js applications with built-in load balancing, monitoring, multi-host deployment, and a graphical console
•Forever - Forever is a simple CLI tool for ensuring that a given script runs continuously (forever). Its simple interface makes it ideal for running smaller deployments of Node apps and scripts.

*Erlang/OTP - http://www.erlang.org/*
•Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability. Some of its uses are in telecoms, banking, e-commerce, computer telephony and instant messaging. Erlang's runtime system has built-in support for concurrency, distribution and fault tolerance.
•OTP is set of Erlang libraries and design principles providing middle-ware to develop these systems. It includes its own distributed database, applications to interface towards other languages, debugging and release handling tools.
•Erlang is a programming language originally developed at the Ericsson Computer Science Laboratory. OTP (Open Telecom Platform) is a collection of middleware and libraries in Erlang. Erlang/OTP has been battle tested in a number of Ericsson products for building robust fault-tolerant distributed applications, for example AXD301 (ATM switch). Erlang/OTP is currently maintained by the Erlang/OTP unit at Ericsson.

*NkSIP - https://github.com/NetComposer/nksip*
•NkSIP is an Erlang SIP framework or application server, which greatly facilitates the development of robust and scalable server-side SIP applications like proxy, registrar, redirect or outbound servers, B2BUAs, SBCs or load generators. NkSIP takes care of much of the SIP complexity, while allowing full access to requests and responses.


#T2.3
**¿Cómo analizar el nivel de carga de cada uno de los subsistemas en el servidor? Buscar herramientas y aprender a usarlas.**

•*PageSpeed Insights by Google* - PageSpeed Insights es una herramienta de Google para analizar y evaluar la velocidad de carga de una páginas web y, lo más importante, además proporcionar una serie de utilísimas sugerencias y herramientas asociadas para mejorar esta velocidad de carga.
•*LoadImpact* - permite medir la carga de usuarios simultáneos que puede soportar tu alojamiento web.
•*LoadComplete* - LoadComplete is a load testing tool for creating and running automated load tests for web servers and services. It will help you check your web server’s performance under a massive load, determine its robustness and estimate its scalability.  Load testing consists in simulating a massive load (requests) on a web server. LoadComplete automates creating load tests byrecording actions you perform over web pages and simulating these actions with dozens and hundreds of virtual users working simultaneously. Each virtual user simulates a recorded scenario, and the entire load test simulates a real-life massive load on the server. LoadComplete produces detailed test results for generated traffic. You can also monitor various server metrics (like CPU usage) during the test run.
•*TestingWhiz* – TestingWhiz’s automated database testing solution offers intuitive ways to test and validate end-to-end databases overcoming the impediments of traditional database testing.
•*Ganglia*  - Ganglia is a scalable distributed monitoring system for high-performance computing systems such as clusters and Grids.

#T2.4
**En este ejercicio debemos buscar diferentes tipos de productos: (1) Buscar ejemplos de balanceadores software y hardware (productos comerciales). (2) Buscar productos comerciales para servidores de aplicaciones. (3) Buscar productos comerciales para servidores de almacenamiento.**

*Balanceadores*

Software:
•	Linux Virtual Server
•	Pound 
•	Pen
•	HAProxy

Hardware:
•	Familia LoadMaster 
•	WebMux Load Balancing de CAI Networks
•	Big IP Local Traffic Manager de F5
•	Barracuda Load Balancer de Barracuda Networks
•	Cisco Arrowpoint

*Servidores de aplicaciones*

•	BEA WebLogic
•	IBM WebSphere
•	Sun–Netscape IPlanet
•	Oracle IAS

*Servidores de almacenamiento*

•	Servidores NAS
•	Servidor de almacenamiento HP ProLiant DL180 




