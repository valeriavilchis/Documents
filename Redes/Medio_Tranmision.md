# Medio de Transmisión

## Introducción

La transmision de datos, es la transferencia de datos de un dispositivo a otro, mediante un medio de transmision, esta transferencía puede ser por un medio guiado y no guiado.

### Medio Guiado

La transferencia de datos, se realiza mediante un medio fisico, generalmente se utiliza el cable de cobre para transmitir señales electricas y la fibra optica para señales opticas.  
El cable de cobre, es el más utilizado en la actualidad, por ser maleable,por su conductividades y ductibilidad.

#### Tipos Principales

1. Palelo: Los cables paralelos no van trenzados (2 hilos de cobre), que son cubiertos por un material aislante, generalmente de plastico, generalmente este tipo de clabeado se utiliza como línea telefónica para transmitir voz.
   1. Su conector es conocido como RJ-11
2. Coaxial: este cable, esta cubierto por un plastico resistente, mientras que en el centro tiene un cable conductor de cobre, y despues de un plastico aislante, el cual se envuelve por una hoja de metal con una malla de cobre trenzado delgado, esta construccion favorece el ancho de banda.  La velocidad de transmision depende de su longitud.  Por ejemplo:  en cables de 1km, se pueden obtener velocidades entre 1 y 2 gigabytes por segundo.  Principalmente es usado para la television y para tramos locales de ciertos tipos de lineas telefonicas.  El conecto que utiliza se llama BNC.
   1. Tipos de cables coaxiales:
   <image src="img/coaxiales.png" alt="Tipos Coaxiales">
3. Par Trenzado: esta formado por pares de hilos de cobre trenzados, los cuales son necesarios para transmitir una señal electrica, el entrelzara dichos cables, reduce las interferencias electricas.  Cada trenza, esta compuesto por 2 hilos de cobre.
   1. Existen dos tipos de par trenzado:
      1. UTP: conector RJ-45, este tipo de cable es el más empleado en redes de área local, por lo económico que resulta para la transmision de datos. (4 pares de hilos trenzados, cubierto cada par, por plastico de diferente color con base en su funcionalidad, y al exterior esta cubierto de otra funda plástica.)
      2. Clasificación de los cables UTP:
        <image src="img/utp_categorias.png" alt="Categorías UTP">
      3. STP: conector RJ-45, es semejante al UTP, 4 pares trenzados de hilos de cobre, la diferencia es que cada para esta cubierto por un material metalico que reduce interferencias, incrementa su inmunidad ante el ruido electrico y las interferencias.  Las desventajas que posee, es que se incremeneta su costo y se dificulta su instalacion.
4. Fibra Optica: usa las ondas de luz para la transmision de la información y se le llama luz infraroja, este cable transforma la luz detectada en pulsos electricos, la luz emisora puede ser de luz o laser.  Cada hilo esta constituido por un nucleo de vidrio o plástico con un revestimiento que permite preservar la luz en su interior.
   1. Clasificación de fibra óptica (clasificación de transmision):
      1. Simplex: se le puede enviar informacion en un solo sentido.
      2. Full Duplex: se utilizan dos cables de fibra optica, esta configuración se utiliza mucho en redes LAN, empleando la emisión de luz LED y alcanza una distancia máxima de cable de 2km.  
Tambien existen cables, cuyas fibras se agrupan en pequeños mazos, y este grupo se encuentra protegido por otro plastico, el cual no permite la penetracion externa de los rayos de luz. Este tipo de clabeado es empleado principalmente en redes WAN y troncales de redes LAN.  Empleando una emision laser, tiene un alcance de de cable de 10KM.
<image src="img/fibra_optica.png" alt="Fibra Óptica">

### Medio No Guiado

Los medios no guiados ocupan el aire como medio de transferencia, para el envio de datos mediante ondas electromagneticas.  
Tambien es conocido como comunicación inalambrica.

#### Tipos Principales

Tambien conocidos como medios inalambricos.

1. Radiofrecuencia: un rango de frecuencia utilizado en las telecomunicaciones que viajan en un espectro electromagnetico.
   1. Rango de frecuencia: 3KHZ a 300GHZ, dicho rango abarca a las ondas de radio, las ondas de radio son faciles de generar, recorren distancias largas, en todas las direcciones desde la fuente emisora, su rango de frecuencia es de 10 KHZ a 300MHZ.
   2. Clasificaciones de ondas de radio:
      1. Baja frecuencia: en su recorrido, sigue la curvatura de la tierra, pero en su ancho de banda solo permite velocidades de transmision bajas.
<image src="img/baja_frecuencia.png" alt="Baja Frecuencia">
      1. Alta frecuencia: son ondas que absorve la tierra, son enviadas a la ionosfera, donde son reflejadas y vueltas de nuevo para una transmision a largas distancias.
<image src="img/alta_frecuencia.png" alt="Alta Frecuencia">
1. Microondas: permite transmisiones terrestres, como satelitales, sus frecuencias comprenden entre los 300MHZ y 300GHZ.  Las microondas no atraviesan bien los obstaculos, razon por la cual es necesario involucrar la instalacion de antenas repetidoras cuando se requiere la comunicacion a largas distancias.  Este tipo de transmision es el que más se emplea en las comunicaciones en redes telematicas e inalambricas.
2. Satélite: es la transmision de microondas pero fuera de la tierra, con ayuda de un satelite espacial, debido a esto es que existe un pequeño retardo en la transmision.  La señal tarda aprox 0.3s en llegar y volver.
3. Infrarrojas: son empleadas principalmente en la comunicacion de corto alcance, como el ejemplo de controles de television, y en general de dispositivos electronicos.  Son economicos en su construccion y direccionales, sin embargo, dichas ondas no puedes transpasar objetos solidos, (esto se considera ventaja en sentido de seguridad. ).  Ademmas el uso de la frecuencia de los infrarrojos no esta regulado por las administraciones de telecomunicaciones y energia.