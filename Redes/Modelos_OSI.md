# Modelos de Red

## Modelos OSI

El nombre del modelo OSI, viene de las siglas "OSI, Open System Interconection o interconexion de sistemas abiertos, este es un modelo desarrollado por la ISO, es el prceso en una representacion abstracta de comunicacion por la red.  
Los modelos de red son representaciones del funcionamiento de una red. **No la red si misma.**  
El __Modelo OSI__ y __Modelo TCP/IP__, son conocidos como modelos de referencia:  
El Modelo OSI divide los proceso de comunicación de una red, en 7 capas logicas:  
7. Aplicación: provee servicos para las aplicaciones que el usuario final necesita.  
6. Presentación: define el formato de los datos que las aplicaciones utlizan.  
5.  Sesión: administra las sesiones de los usuarios.  
4. Transporte: establece los segmentos de datos en la fuente de datos, de transferirlos y de reensamblarlos en el host destino.  
3. Red: crea y establece la dirección de los paquetes de datos para su entrega, haciendo uso de diferentes dispositivos.  
2. Enlace de datos: crea y establace la dirección de las tramas para entregarlas entre los host de una LAN y entre dispositivos de red WAN.  
1. Fisica: transmite datos binarios, gracias a los medios de transmision entre dispositivos.

Es importante mencionar que el proceso de comunicación comienza en la capa de aplicación y termina en la apa física.  

## Modelo TCP/IP

4. Aplicación: representa los datos para los usuarios.  (4)
3. Transporte: comunica a los diferentes dispositivos, ademas de llevar a cabo un proceso de correcion de errores.  (3)
2. Internet: encntrar la mejor ruta en la red para enviar los datos. (2)
1. Acceso a red: controla los dispositivos y medios de transmision. (1)

## Comparación Modelo OSI vs TCP/IP  
<image src="img/osi_tcp-ip.png" alt="OSI vs TCP/IP">

**El nucleo del proceso de una red, recide enlas capas de transporte y de red.**  
- En la capa de transporte es donde opera el modelo tcp/ip (Protocolo de control de transmision).  
- En la capa de transporte funciona el IP (Protocolo de internet)

## Unidad de datos de protocolo. (PDU)  

Se refiere al nombre que los datos reciben en cada capa del modelo de referencia TCP/IP.  
Dependiendo del nivel de capa del modelo TCP/IP, los datos se nombrarn de cierta manera.  
<image src="img/pdu.png" alt="PDU">

## Comité 802 DE LA IEEE

Los estándares IEEE 802.3 e IEEE 802.11 son estándares IEEE importantes en redes de computadoras.  
El estándar IEEE 802.3 define el control de acceso al medio (MAC) para Ethernet por cable. Esta tecnología generalmente es para las LAN, pero también tiene aplicaciones para redes de área extensa (WAN).
<image src="img/estandar_ieee.png" alt="Estandar IEEE">