# Blue-Team
Informe de Infraestructura de Red
En este proyecto, se ha configurado una infraestructura de red utilizando máquinas virtuales de Kali Linux y Windows, gestionadas a través de pfSense. A continuación, se detallan los pasos y componentes principales:

1.Configuración de pfSense:
Se ha instalado pfSense en una máquina virtual para actuar como firewall y router.
Se han configurado dos interfaces de red en pfSense: una para la red interna (LAN) y otra para la red externa (WAN).

2.Red DMZ con Honeypot Cowrie:
En la máquina virtual de Kali Linux, se ha creado una red DMZ.
Dentro de esta DMZ, se ha desplegado un honeypot Cowrie para simular un entorno vulnerable y atraer posibles atacantes.

3.Red DMZ2 con Servidor Apache:
También en la máquina virtual de Kali Linux, se ha configurado una segunda DMZ (DMZ2).
En esta DMZ2, se ha instalado y configurado un servidor Apache para alojar aplicaciones web.

4.Red LAN con Máquina Windows:
En la red LAN, se ha desplegado una máquina virtual con Windows.
Esta máquina se utiliza para tareas administrativas y de usuario final dentro de la red interna.

5.Envío de Logs a Elastic Cloud:
Todos los logs generados por las diferentes máquinas y servicios (incluyendo Windows, Cowrie, y Apache) se envían a un servidor de Elastic Cloud.
Elastic Cloud se utiliza para centralizar, analizar y visualizar los logs, facilitando la monitorización y detección de incidentes de seguridad.
Esta configuración permite una gestión eficiente y segura de la red, con capacidades avanzadas de monitorización y análisis de logs.
