# Dispositivos de red

## Definicion

Un dispositivo es un equipo tecnologico que conecta segmentos de red.  
Los dispositivos estan divididos en dos categorias generales: dispositivos de usuario final y dispositivos de red.

## Dispositivos de usuario final

Los dispositivos de usuario final proveen servicios a un usuario final, por ejemplo: computadoras, escaneres, impresoras, etc.  
Los dispositivos de usuario final que proveen una conexión a la red son llamados hosts.

## Dispositivos de red

Los dispositivos de red son todos aquellos que conectan a los dispositivos de usuario final a la red, tales como: repetidores, hubs, puentes, sqitches y routers.

## Dispositivos de la capa física

- Repetidores: 
Su objetivo es regenerar y resincronizar las señales al nivel de bits para permitir que viajen largas distancias.  
<image src="img/repetidores.png" alt="Repetidores">
- Hubs: Tienen un funcionamiento similar al de los repetidores, sin embargo, ademas de regenerar y resincronizar las señales al nivel de bits, funcionan como un punto central de conexion para varios hosts.  
__Tambien son conocidos como repetidores multipuerto.__
<image src="img/hubs.png" alt="Hubs">

## Dispositivos de la capa de enlace de datos

- Tarjeta de interface de red (NIC): "Network Interface Card", provee una conexión física a la red para un host.  
Toda NIC y dispositivio de red tiene asignado un código único llamado dirección MAC (Media Access Control o Control de Accesos a Medios).  
La direccion MAC permite controlar el acceso de un host a los medios.  
<image src="img/nic.png" alt="NIC">
- Puentes: diseñado para crear dos o más segmentos de red. Su proposito es filtrar el tráfico en una LAN, lo cual, hace que se mantenga un tráfico en un segmento, pero a la vez, se puede comunicar con otro.  
Los puentes filtran el tráfico de la red a través de la dirección MAC.  
<image src="img/puentes.png" alt="Puentes">

## Dispositivos de Red
- Switches: tiene un proposito similar a los puentes.  
Debido a que la comunicacion de datos de un switch son más rápidos que los hubs que realizan una conmutación en software.  
Cada puerto de un switch actúa como un puente separado.  
<image src="img/switches.png" alt="Switches">

- Routers: pasa paquetes de datos entre redes, todo esto basandose en un direccionamiento lógico.  
Toman decisiones acerca de la mejor ruta para entregar los paquetes en la red. Puede conectar diferentes tecnologías de la capa de enlace de datos.  
__Los routers son la columna vertebral de internet debido a que trabajan con el protocolo de internet IP.__  
<image src="img/router.png" alt="Router">

## Dispositivos de capas superiores

- Firewalls: protege los recursos de una red de los usuarios.