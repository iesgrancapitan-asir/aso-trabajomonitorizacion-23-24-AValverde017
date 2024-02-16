# MONITORIZACIÓN CON NAGIOS

# 1  Las herramientas de monitorización de servidores.
       
## 1.1  Introducción general
En el mundo dinámico de la gestión de servidores, contar con herramientas eficaces de monitorización es esencial para garantizar un rendimiento óptimo y una disponibilidad constante
Desde la detección temprana de problemas hasta la optimización de recursos, estas herramientas desempeñan un papel crucial en la administración de infraestructuras de TI.
A continuación, se presentan cinco herramientas destacadas, cada una con su enfoque único en la monitorización de servidores

## 1.2  Las herramientas  a estudiar
   - **Nagios** :

Nagios es una de las herramientas de monitorización de código abierto más populares y de larga data.

Ofrece una amplia gama de capacidades de monitorización, incluyendo la supervisión de servicios de red, recursos de hardware, aplicaciones y más.

Nagios es altamente personalizable y extensible, lo que permite a los usuarios adaptar la solución a sus necesidades específicas.

Además, su capacidad para generar alertas proactivas ante problemas críticos garantiza una respuesta rápida a las incidencias del servidor.

- **Zabbix** :

Es una plataforma de monitorización empresarial que proporciona una visión integral del rendimiento de la infraestructura de TI.

Con capacidades de monitorización en tiempo real, Zabbix permite supervisar servidores, redes y servicios en un solo tablero unificado.

Su arquitectura distribuida y escalable lo hace ideal para entornos de gran tamaño.

Zabbix también ofrece funciones avanzadas de informes y visualización de datos para un análisis detallado del rendimiento del servidor.

- **Prometheus:**

Prometheus es una herramienta de código abierto diseñada específicamente para la monitorización de sistemas y servicios en entornos de nube. Utiliza un modelo de datos multidimensional y una consulta flexible para recopilar y almacenar métricas de forma eficiente.

Además, Prometheus ofrece integración con herramientas de alerta como Alertmanager, lo que facilita la detección temprana de problemas y la respuesta proactiva.

Su arquitectura modular y su capacidad para escalar horizontalmente hacen que sea una opción popular para entornos en crecimiento.

- **SolarWinds Server & Application Monitor (SAM):**

SAM es una solución integral de monitorización de servidores y aplicaciones desarrollada por SolarWinds, un líder en herramientas de gestión de TI. SAM ofrece monitoreo en tiempo real de servidores físicos, virtuales y en la nube, junto con una amplia gama de aplicaciones y servicios.

Su interfaz intuitiva y sus capacidades de automatización simplifican la configuración y el mantenimiento del sistema de monitorización.

Además, SAM proporciona informes detallados y análisis de tendencias para optimizar el rendimiento y la disponibilidad del servidor.


 # 2  La herramienta NAGIOS 
 ## 2.1  Historia
 Nagios, nació en 1999 como un proyecto personal de Ethan Galstad. La motivación detrás de este proyecto fue la necesidad de supervisar y rastrear el estado de múltiples servidores y servicios dentro de la red de la Universidad de Minnesota, donde Galstad trabajaba en ese momento.

Inicialmente, NetSaint se centraba en la monitorización básica de servicios de red y notificará a los administradores cuando se detectan problemas. A medida que el proyecto evolucionó y ganó popularidad en la comunidad de código abierto, Galstad decidió renombrarlo como "Nagios" en 2002, un acrónimo recursivo que significa "Nagios Ain't Gonna Insist On Sainthood" (Nagios no va a insistir en ser santo), reflejando la actitud pragmática y flexible del proyecto.

Durante la década de 2000, Nagios se consolidó como una solución líder en monitorización de infraestructuras de TI, ganando una amplia base de usuarios en todo el mundo, desde pequeñas empresas hasta grandes corporaciones. 

La flexibilidad y extensibilidad de Nagios, facilitada por su arquitectura modular y su sólido soporte de complementos y extensiones, lo convirtieron en una opción popular para adaptarse a una variedad de casos de uso y entornos de TI.

En la actualidad, Nagios sigue siendo una herramienta fundamental en la caja de herramientas de los administradores de sistemas y equipos de operaciones de TI. Su comunidad activa de usuarios y desarrolladores continúa contribuyendo con mejoras y nuevas características, manteniendo viva la evolución del proyecto.

Trayectoria a través de los años:

2004: Se lanza la versión 2.0 de Nagios, introduciendo una interfaz web y un sistema de plugins modular.
2005: Nagios se convierte en uno de los proyectos de código abierto más populares en SourceForge.
2008: Se lanza la versión 3.0 de Nagios, con mejoras en la escalabilidad, la seguridad y la gestión de usuarios.
2012: Se lanza Nagios XI, una versión comercial con soporte técnico y características adicionales.
2017: Se lanza Nagios Core 4.0, una versión mayor con mejoras significativas en la arquitectura y el rendimiento.
2023: Nagios continúa siendo una herramienta de monitorización de servidores líder en el mercado, con una comunidad activa de usuarios y desarrolladores.
 ## 2.2  Funciones/utilidades y características. Ventajas y desventajas
Su principal aplicación consiste en la vigilancia y monitorización de equipos y servicios. El programa envía avisos y alertas cuando el comportamiento de los equipos y servicios no es el que debería.

El envío de notificaciones de alerta puede ser realizado por varios medios: mensajes de texto, mensajes instantáneos o correo electrónico.

Se adapta a entornos de pequeña y gran escala. Permite la monitorización desde unas decenas hasta miles de dispositivos y servicios.

Proporciona una interfaz intuitiva que permite una configuración sencilla y una visualización de estados e informes limpia.

Posee gran cantidad de opciones de personalización. A través de sus plugins se pueden monitorear servicios específicos

 ## 2.3  Plataformas posibles donde instalar:
### A. Agentes:
Los agentes de Nagios se pueden instalar en una amplia variedad de plataformas, incluyendo:
- Sistemas operativos:
  
   - Linux (Debian, Ubuntu, CentOS, Red Hat, etc.)
   - Windows (Server, Professional, etc.)
   - macOS
   - FreeBSD
   - Solaris
   - AIX
- Dispositivos de red:
   - Routers
   - Switches
   - Firewalls
- Aplicaciones:
   - Servidores web (Apache, Nginx, etc.)
   - Bases de datos (MySQL, PostgreSQL, etc.)
   - Aplicaciones de correo electrónico (Exchange, Zimbra, etc.)
### B. Máquinas desde las que se monitoriza:
Nagios se puede instalar y ejecutar en una variedad de plataformas para la monitorización, incluyendo:
- Servidores Linux:
   - Debian
   - Ubuntu
   - CentOS
   - Red Hat
   - SUSE
- Servidores Windows:
   - Server 2012
   - Server 2016
   - Server 2019
- Servidores macOS:
   - macOS 10.12 Sierra
   - macOS 10.13 High Sierra
   - macOS 10.14 Mojave
   - macOS 10.15 Catalina
- Servidores FreeBSD:
   - FreeBSD 11.x
   - FreeBSD 12.x
- Servidores Solaris:
   - Solaris 11
   - Solaris 12
### C. Sistemas y distribuciones con versiones necesarias:
La versión de Nagios que necesita dependerá de la plataforma en la que la instale. A continuación se muestran algunos ejemplos:
- Nagios Core 4.x:
    - Linux: Debian 9 ("Stretch"), Ubuntu 16.04 ("Xenial Xerus"), CentOS 7 ("El Capitan"), Red Hat Enterprise Linux 7 ("Maipo")
    - Windows: Server 2012, Server 2016
    - macOS: 10.12 Sierra
    - FreeBSD: 11.x
    - Solaris: 11
- Nagios XI:
   - Linux: Debian 9 ("Stretch"), Ubuntu 16.04 ("Xenial Xerus"), CentOS 7 ("El Capitan"), Red Hat Enterprise Linux 7 ("Maipo")
   - Windows: Server 2012, Server 2016
   - macOS: 10.12 Sierra
 
 ## 2.4  Requisitos de agentes y de máquinas de monitoreo
 **Requisitos previos:**

**Sistema operativo** : Nagios es compatible con una amplia gama de distribuciones de Linux, como Debian, Ubuntu, CentOS, Red Hat Enterprise Linux (RHEL), Fedora, openSUSE, entre otros.

**Pasos para la instalación:**

**Actualización del sistema:**

Antes de comenzar la instalación, es recomendable actualizar el sistema operativo a su última versión.

**Instalación de dependencias básicas:**

Los requisitos básicos incluyen paquetes esenciales y herramientas necesarias para compilar y ejecutar Nagios Core y sus complementos.

_sudo apt install gcc glibc glibc-common wget unzip httpd php gd gd-devel perl postfix_

**Creación de un usuario y un grupo para Nagios:**

Este paso es necesario para asegurar que Nagios tenga los permisos adecuados.

_sudo useradd -m -s /bin/bash nagios_

_sudo groupadd nagcmd_

_sudo usermod -a -G nagcmd nagios_

_sudo usermod -a -G nagcmd apache_

**Descarga de Nagios Core:**

_wget https://github.com/NagiosEnterprises/nagioscore/archive/nagios-x.x.x.tar.gz_

**Descarga e instalación de Nagios Plugins:**

Los plugins de Nagios son esenciales para realizar las comprobaciones de los servicios y recursos que deseas monitorear.

_wget https://nagios-plugins.org/download/nagios-plugins-x.x.x.tar.gz_

**Descarga e instalación de NRPE (Nagios Remote Plugin Executor):**

NRPE es necesario si deseas realizar comprobaciones en sistemas remotos.

_wget https://github.com/NagiosEnterprises/nrpe/releases/download/nrpe-x.x.x/nrpe-x.x.x.tar.gz_

**Compilación e instalación de Nagios Core:**

Después de descargar el archivo tar, descomprímelo y sigue las instrucciones de compilación e instalación, que son similares a las proporcionadas en la instalación de Nagios Core en los pasos anteriores.

**Compilación e instalación de Nagios Plugins y NRPE:**

Después de descargar los archivos tar de Nagios Plugins y NRPE, descomprimirlos y sigue las instrucciones de compilación e instalación proporcionadas en sus respectivas documentaciones.

**Configuración adicional:**

Una vez que hayas instalado Nagios Core, Plugins y NRPE, necesitarás configurarlos adecuadamente para tus necesidades específicas de monitoreo. Esto incluye definir los hosts y servicios que deseas monitorear, establecer las notificaciones, etc.


 ## 2.5  Esquema de Red 
 Antes de proceder a las pruebas con Nagios, debemos de crear un esquema de red del escenario que vamos a desplegar. En nuestro caso, es escenario lo vamos a desplegar en el Servidor Luna de nuestro instituto; y es el siguiente esquema de red:

![Esquema de red](./capturas/esquema%20de%20red.png)

El escenario va a estar compuesto por un Ubuntu 22.04.3 LTS que tiene la ip 192.168.12.218/24; esta máquina es la que va a ser monitorizada. En esta máquina se instalará el paquete "nagios3 nagios-nrpe-plugin" .

Por otro lado, tenemos un cliente Ubuntu Server 22.04.3 LTS con ip 192.168.12.219/24; esta máquina es la que va a monitorizar al Ubuntu Cliente. En esta máquina se instalará el paquete "nagios-nrpe-server" para la monitorización remota del Ubuntu Cliente.


# 3. Instalación y configuración en máquinas a monitorizar (agentes) y remotas
 ### /////NOTA: EL PROCESO DE INSTALACIÓN Y LA PUESTA EN MARCHA DE PRUABAS SERÁ EXPUESTO A MODO DE CAPTURAS///
 ## 3.1  Instalación y configuración en agentes 

 Como dijimos anteriormente, la máquina de Ubuntu Server es la que va a monitorizar al cliente Ubuntu, con lo cual el Ubuntu Server será también nuestro Nagios Server.

![](./capturas/instalacion%201.png)

![](./capturas/instalacion%202.png)

![](./capturas/instalacion%203.png)

![](./capturas/instalacion%204.png)


Si ponemos en el navegador ‘http://ipservidor/nagios’ nos debería de entrar en nagios, nos pedirá también un usuario y contraseña que es la que hemos configurado al principio de la instalación. Como vemos, también nos sale el la máquina donde tenemos instalados el Nagios Server, eso es porque Nagios también monitoriza algunos servicios de esta máquina.

![](./capturas/nagios%20nav.png)

 ## 3.2  Diseño de pruebas

 En este caso, desde nuestro Servidor Nagios vamos a monitorear ciertos servicos de nuestro agente Nagios. Los servicios a monitorear son el espacio en disco, la conectividad (ping), el servicio ssh, el servidor web (http), las actualizaciones y usuarios conectados al agente. 
 ## 3.3  Puesta en marcha de pruebas

 ![p1](./capturas/pruebas%201.png)
 ![p2](./capturas/pruebas%202.png)
 ![p3](./capturas/pruebas%203.png)
 ![p4](./capturas/pruebas%204.png)

 # 4  Otros puntos a investigar según la herramienta

En el transcurso de la realización de este trabajo hemos investigado sobre otros usos que se le puede dar a la herramienta nagios y hemos encontrado lo siguientes

**Instalación mediante script en las máquinas de la red a monitorizar:**

- En Nagios es posible automatizar la instalación en Linux utilizando scripts o herramientas de automatización como Ansible, Puppet o Chef. Esto facilita la implementación en grandes redes.

**Monitorización remota por SSH o en consola:**

- En Nagios se pueden monitorizar servidores remotos tanto en Linux como en Windows usando SSH o WMI (Windows Management Instrumentation).

**Monitorización usando el navegador web. Alerta a usuario:**

- Nagios ofrece una interfaz web llamada Nagios XI que permite la monitorización y la configuración de alertas.

- Las alertas son personalizables y pueden enviarse por correo electrónico, SMS, notificaciones push, webhooks y otros métodos.

**Tarea programada en cron:**

- Nagios utiliza cronjobs en Linux para programar la ejecución de plugins de monitorización y la generación de informes.

 # 5  Conclusiones y problemas encontrados 
Este trabajo se ha basado en la implementación y configuración de la herramienta de monitorización Nagios en un entorno de red.

En el desarrollo de la misma no encontramos ningún problema a la hora de la utilización del software, configuración del mismo o en la parte de investigación

Se realizó la instalación de Nagios en un servidor Ubuntu Server 22.04.3 LTS, que actúa como Nagios Server, y se configuró para monitorizar un cliente Ubuntu 22.04.3 LTS.

En el transcurso de la práctica hemos llegado a unas conclusiones las cuales serían:

- Nagios es una herramienta poderosa y flexible para la monitorización de servidores y redes.
- La instalación y configuración de Nagios puede ser compleja, pero existen recursos disponibles para facilitar el proceso.
- La monitorización de servidores y redes es una tarea esencial para garantizar la disponibilidad y el rendimiento de los sistemas informáticos.

En general, este trabajo ha demostrado que Nagios es una herramienta efectiva para la monitorización de servidores y redes. La implementación y configuración de Nagios puede ser un desafío, pero los beneficios de la monitorización proactiva son significativos.

 # 6 Bibliografía

[https://howtoforge.es/como-instalar-el-software-de-monitorizacion-nagios-en-ubuntu-18-04-lts/](https://howtoforge.es/como-instalar-el-software-de-monitorizacion-nagios-en-ubuntu-18-04-lts/)

[https://www.nagios.org/documentation/](https://www.nagios.org/documentation/)

[https://support.nagios.com/kb/article.php?id=60](https://support.nagios.com/kb/article.php?id=60)

[https://www.youtube.com/live/hCZQp24-kCA?si=EfKOTdhcgNUc8CPp](https://www.youtube.com/live/hCZQp24-kCA?si=EfKOTdhcgNUc8CPp)


# ANEXO. Desarrollo del proyecto con SCRUM
## I. Equipo y roles
- **Equipo:** The Scrumest
- **Miembros y Roles:** Cinthia Castro (Instalación y Pruebas), Ángel Ordoñez (Investigación y fallos) y Antonio Valverde (ScrumMaster)

## II. Reuniones realizadas 
- 9/2 Sprint 1
- 12/2 Sprint 2
- 15/2 Sprint 3
## III. Documentos: 
- link al backlog del equipo  [https://docs.google.com/spreadsheets/d/1dEuorknY3bLKmN2ouG2tsG-goTInmJsRizUGxh-Q2f8/edit#gid=1743950190](https://docs.google.com/spreadsheets/d/1dEuorknY3bLKmN2ouG2tsG-goTInmJsRizUGxh-Q2f8/edit#gid=1743950190)

           
           
