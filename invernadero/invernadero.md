
## Introducción
Se documenta la implementación de un invernadero inteligente, utilizando Arduino y RaspBerry PI.

## Agradecimientos
Extendemos un agradecimiento al Dr. Carlos Omar Gonzaléz Morán,
profesor de tiempo completo e investigador
de la Universidad Autónoma del estado de México,
Centro Universitario Valle de México, por proporcionarnos el contacto
con Ing. Crystian Pichardo González, jefe del departamento de
nutrición del DIF Tlalnepantla, Estado de México, con el cual se
desarrollo el Invernadero Inteligente expuesto en este documento.

Agradecemos al Ing. Christian por la confianza y permitir agregarnos
a su grupo de trabajo y proyecto de invernadero inteligente.

Agradecemos al DIF (Sistema Nacional para el Desarrollo Integral
de la Familia) del Estado de México con ubicación en Av.
Convento de Santa Mónica s/n , esq. Convento de San Fernando,
Fraccionamiento Jardines de Santa Mónica, Tlalnepantla de Baz,
Estado de México, por prestar un espacio para la instalación del invernadero.

Agradecemos a la compañía de hardware y software libre Arduino,
ya que la plataforma Arduino es parte fundamental de este invernadero inteligente.

Agradecemos a la compañía Raspberry Pi, ya que el control de los Arduinos
y tratamiento de los datos mediante Raspberry Pi es pieza clave en el invernadero inteligente.

Agradecemos totalmente a  la Universidad Autónoma del Estado de México,
en especial al Centro Universitario Valle de México, ya que en este espacio
académico se logro planear gran parte del invernadero inteligente.


## Invernadero
Parte fundamental de este trabajo esta relacionado con los invernaderos, a continuación se describe lo que es un invernadero así como sus características y funciones, un invernadero necesita manejar adecuadamente temperaturas de ambiente y suelo, mantener bajo control estas variables de medición garantizan aprovechar todos los beneficios que un invernadero proporciona.

### Definición de Invernadero
Un invernadero es aquella estructura cerrada, el nivel de tecnificación con el que cuente es de acuerdo a las necesidades que se necesiten cubrir, mantener una producción alta es el objetivo principal de un invernadero [(C. Marín, M., 2013)](#MAR2013).

Parte de la estructura del invernadero  se encuentra cubierta por materiales que permiten la entrada de los rayos del sol, esto provoca una ambiente artificial, optimo para el cultivo de plantas [(Miserendino E. ,Astorquizaga R., 2014)](#MiseAsto2014).

Los invernaderos se encuentran clasificados en:

1. Invernaderos planos o tipo parral
1. Invernadero en raspa y amagado
1. Invernadero asimétrico
1. Invernaderos de capilla
1. Invernaderos de doble capilla
1. Invernadero túnel o semicilíndrico

### Invernaderos planos o tipo parral

La implementación de este tipo es en zonas con poco lluvia, su construcción se encuentra en dos partes, estructura vertical y horizontal.

La estructura vertical está constituida por soportes rígidos con funciones perimetrales o interiores, los soportes internos se encuentran a una distancia de 2x2 o 3x4 metros entre si, los soportes perimetrales cuentan con una inclinación de 30 grados hacia el exterior respecto a su vertical, mismos que tienen una separación de 2 a 1.5 metros, el material de estos soportes puede ser tubos de acero, o puntales de madera. En la estructura horizontal encontramos dos mallas de alambre galvanizado superpuestas, estas mallas ayudan al soporte de laminas de plástico. Todos los soportes verticales se encuentran fijados a suelo mediante zapatas de concreto, estos bloques están dentro de pozos para cimentación [(Agroinformación. Tipos de invernaderos, 2019)](#AGR2019).

### Invernadero en raspa y amagado

Los invernaderos de raspa y amagado son resultado de una transformación de los invernaderos planos o tipo parral cuya modificación se presenta en la forma de tratar el agua de la lluvia, ya que en un invernadero plano la lluvia puede provocar estragos en el invernadero [(Invernaderos Raspa y Amagado - Parral - Almería, 2019)](#NOVA2019).

Estos se encuentran sujetados al suelo mediante tubos galvanizados con alambres "raspa", y la parte baja "amagado", unidas mediante horquillas, mismas en las que se encuentran los canales para flujo del agua de lluvia [(Invernaderos de raspa y amagado,  2019)](#INF2019).

### Invernadero asimetrico

Este mantiene una geometría asimétrica, unos de sus lados se encuentra con una mayor inclinación que el otro lado, dicha inclinación es a partir de un estudio de la incidencia perpendicular de la luz solar a medio día en el invernadero, durante invierno estos cuentan con un alto aprovechamiento de la radiación solar
[(Principales Tipos de Invernaderos, 2019)](#HOR2019).

En la construcción de este tipo de invernaderos, el ángulo de inclinación esta cerca a 60° grados, esta inclinación impacta en un daño estructural, ya que los fuertes vientos provocan modificaciones en este mismo, sin embargo mediante modificaciones tanto de lado bajo y las cubiertas, puede solucionarse un poco dichos problemas, pero el aprovechar totalmente la radiación solar, incluso en estaciones del año con radiación solar escala, los vuelve muy atractivos para su implementación, detalles como la ventilación son resueltos mediante aperturas tanto en el cetro o arcos de las partes superiores [(Invernadero tipo asimetrico o inacral: diseños y tamaños, 2019)](#ELJ2019).

### Invernadero de capilla

 Este es empleado por compañias para el cultivo de flores, mantiene una pendiente (cambio) en la parte superior, siendo variable según la radiación y niveles de lluvia, medidas de ancho van de 6 y 12 metros, altura de 2 a 2.5 metros
 [(Hernandez & Alvarez, 2019)](#HA2016).

 Este invernadero también conocido como multicapilla, cuenta con arcos y con una estructura total metálica, su distinción se debe a su forma dada por los arcos en la parte superior.

 En medidas dado un estándar son:

 - Ancho: 8 m - 9.60 m.
 - Altura Bajo Canal: 4 m - 5 m – 5.50 m.
 - Altura al zenit: 5.80 m - 6.30 m - 6.80 m.
 - Separación entre pilares: 5 m (interior) – 2,50 m (exterior).

### Invernadero túnel o semicilíndrico

Compuesto por una serie de arcos paralelos, dando la forma tipo túnel, estos están unidos mediante perfiles cilíndricos, dando rigidez, no cuentan con paredes rectas, su instalación es directo en el suelo, se utilizan con mayor frecuencia en el cultivo de plantas bajo porte, y hortalizas con cuidados menores, sus sistemas de ventilación son frontal [("Invernaderos Túnel - IEP invernaderos", 2019)](#IEP2019).

### Cuidado ambiental


## Internet de las cosas

Los avances en electrónica e informática, han permitido grandes crecimientos para los sistemas de tratamiento de información, el tamaño de microprocesadores, y la diversidad de fabricantes de sensores a precios accesibles, extienden a la creación de Internet de las cosas o conocido también como Internet de los objetos.

Internet de las cosas promete ser la evolución de Internet, cuyas capacidades para la recolección y analizas de información se volverán por de facto las herramientas de sabiduría para la humanidad.

Internet de las cosas no solo consiste en un despliegue de computadores y sensores que estén minando datos, también esta relacionado con las capacidades de relaciones entre gobiernos y empresas, esto para permitir un crecimiento crucial y totalmente satisfactorio, mismas relaciones permitirán resolver problemas como el abastecimiento de energía y extensión de redes para la comunicación y sostenibilidad de sensores y procesadores.
<center>
<img src="http://cabaseiot.com.ar/wp-content/uploads/2019/07/nota-iprofesional.jpg"
 style="width : 450px;"/>
 <br>
 Fuente de image: http://cabaseiot.com.ar
</center>

La aplicación de el Internet de las cosas esta basado en la conexión de dispositivos con los que el ser humano actualmente esta rodeando, esta conexión intercambia información generada por estos mismos, dicha información puede ser para estudio y generar un conocimiento o en la mejor de los casos, para dotar de autonomía a otros dispositivos a partir del cambio y patrones en la información.

Internet de las cosas, es la firma tecnológica que dejara huella de la humanidad en nuestro mundo, **Kevin Ashton** , creador del termino Internet de las Cosas menciona que:

> "*si los libros, termostatos, refrigeradores, paquetería,
lámparas, botiquines, partes automotrices, entre otros, estuvieran conectados a
Internet y equipados con dispositivos de identificación, no existirían, en teoría,
artículos fuera de stock o medicinas caducas; sabríamos exactamente su ubicación,
cómo se consumen en el mundo; el extravío sería cosa del pasado, y sabríamos qué
está encendido y qué está apagado en todo momento. Internet de las cosas tiene el
potencial de cambiar el mundo, como hizo Internet en su momento. Tal vez aún más.*” --Kevin Ashton--


## Arduino

Es un proyecto de código abierto, se basa en el fácil uso de hardware y software, Arduino es una tarjeta para leer y escribir datos provenientes de sensores y actuadores, todo esto a partir de un microcontrolador, el inicio de este proyecto es a apartir del 2005, como un programa para estudiantes en el Interaction Design Institute Ivrea en Ivrea, Italia [("Arduino - Introduction", 2019)](#ARD2019) .

### Características Arduino

Arduino tiene alta presencia en proyectos de electrónica ya que cuenta con las siguientes características:

- Bajo en costos, los precios para su comprar son muy accesibles, tanto para estudiantes y proyectos.
- Multiplataforma, su entorno de desarrollo esta disponible para Windows, Macintosh OSX, y GNU/Linux.
- Ambiente de desarrollo fácil de utilizar y aprender, emplea codigo en C y C++.
- Open Source, es de código abierto
- Diseño Hardware libre, los esquemas para el diseño de una tarjeta arduino estan disponibles.

### IDE Arduino
Para trabajar con Arduino, una de las opciones es medainte el IDE de Arduino:

<center>
<img src="https://www.programoergosum.com/images/cursos/253-curso-de-iniciacion-a-arduino/software-arduino-ide.png"
 style="width : 500px;" />
 <br>
 Fuente de image: https://www.programoergosum.com
</center>

En este IDE las acciones que nos permite realizar son:

- **Verificar:** Al momento de tener código fuente escrito en el editor, esta herramienta
permite analizar el código mediante su compilador, para detectar problemas y violaciones de sintaxis, sintaxis total de lenguaje C y C++, así mismo verifica si se encuentran inicializadas parámetros para la plataforma Arduino.

- **Cargar:** Cuando es el momento de ejecutar nuestro código en la plataforma Arduino, esta herramienta permite subir el código ya compilador al controlador del
Arduino.

- **Nuevo:** Ejecuta una instancia nueva y vacía del IDE Arduino

- **Abrir:** Ejecuta una instancia nueva y con algún proyecto Arduino.

- **Guardar:** Guarda el proyecto Arduino, crea un directorio automatico si este no esta.

- **Monitor Serial:** Quizás sea una de las herramientas fundamentales del IDE Arduino, este permite volcar toda la información en la interfaces de conexión serial entre Arduino y la computadora, se puede leer e incluso escribir directamente en la interfaz serial.

- **Editor:** Edición directa del código fuente del proyecto Arduino.

- **Notificaciones:** En esta parte se puede ver los mensajes del estado de las acciones realizadas en el IDE Arduino, muy útil para corregir los errores en nuestro proyecto.  

### Arduino hardware
La tarjeta Arduino se presenta a continuación:
<center>
<img src="https://www.arduinohobby.com/wp-content/uploads/2018/07/ARDUINO.jpg"
 style="width : 500px;" />
 <br>
 Fuente de image: https://www.arduinohobby.com/
</center>

- **Puerto USB:** Este puerto es la interfaz en la cual se comunica con la computadora, este mismo se emplea para su alimentación, todo el flujo serial se puede realizar mediante este puerto USB.

- **Alimentación externa:** La Alimentación de energía no solo es por USB, este pin se emplea en cuando la tarjeta sera embebida con otros sistemas.

- **Boton Reset:** Al cargar nuestro programa en el microcontrolador de Arduino este comienza a ejecutarse, si requerimos que este se ejecute desde el inicio, el boton reset lo permite.

- **Pines Digitales:** Estos pines están dotados para comunicación digital, tanto para leer y escribir.

- **Led Encendido:** Indica cuando esta alimentado con energía eléctrica la tarjeta Arduino.

- **Pines de Alimentación:** Son de utilidad cuando se requiere alimentar un actuador o sensor.

- **Pines Analógicos:** Estos pines están dotados para comunicación analógica, tanto para leer y escribir.

- **Microcontrolador:** Parte fundamental de Arduino, es el centro de operaciones, el cerebro de Arduino.


## Raspberry PI

### Historia

### Características Raspberry PI

### Lenguaje de programación

## Invernadero Inteligente

### Propósito

### Recursos

#### Hardware

#### Software

## Invernadero caso practico

### Lugar del invernadero

### Propósito de este invernadero

### Necesidad de este invernadero

## Propuesta de invernadero

### Objetivos

### Funcionamiento


## Desarrollo

### Hardware

#### Plataformas

#### Sensores

### Software

#### Programación en arduino

#### Programación en python

#### DashBoard web con angular

#### DashBoard local con python

## Instalación

### Arduino esclavo y maestro

### RaspBerry PI maestro

### Diagrama de instalación

## Trabajando con sensores

### Simulación

### Armado físico

### Instalacion fisica

## Desarrollo del software para Arduino

### Diagramas de flujo Arduino

## Desarrollo del software para RaspBerry PI

### Diagramas de flujo RaspBerry PI

## Conectando software Arduino con RaspBerry PI

## Ejecución de invernadero

### Temperatura ambiente

### Temperatura del suelo

### Humedad del suelo

### Electrovalvula

## Desarrollo futuro

### Otros sensores

### Automatizaciones

### Notas finales

## Referencias
1. <a name="MIS2014"></a> Miserendino E. ,Astorquizaga R. (2014). Invernaderos: aspectos básicos sobre estructura, construcción y condiciones ambientales [Ebook] (p. 1). Retrieved https://inta.gob.ar/sites/default/files/script-tmpinta_agricultura23_invernadero.pdf.

1. <a name="MAR2013"></a>C. Marín, M. (2013). Diseño de Invernaderos [Ebook] (p. 3). Retrieved https://www.portalfruticola.com/assets/uploads/2017/07/Manual-de-Invernaderos-2.pdf.

1. <a name="AGR2019"></a>Agroinformación. Tipos de invernaderos. (2019). Retrieved 9 October 2019, from http://www.abcagro.com/industria_auxiliar/tipo_invernaderos2.asp

1. <a name="NOVA2019"></a>Invernaderos Raspa y Amagado - Parral - Almería. (2019). Retrieved 16 October 2019, from https://www.novagric.com/es/venta-invernaderos-novedades/tipos-de-invernaderos/invernaderos-raspa-amagado

1. <a name="INF2019"></a>Invernaderos de raspa y amagado. (2019). Retrieved 16 October 2019, from https://www.infoagro.com/industria_auxiliar/invernaderos_raspa_amagado.htm

1. <a name="HOR2019"></a>Principales Tipos de Invernaderos. (2019). Retrieved 16 October 2019, from https://www.horticultivos.com/agricultura-protegida/invernaderos/principales-tipos-invernaderos/

1. <a name="ELJ2019"></a>Invernadero tipo asimetrico o inacral: diseños y tamaños. (2019). Retrieved 16 October 2019, from https://www.eljardin.ws/invernaderos/tipos/invernadero-tipo-asimetrico-o-inacral.html

1. <a name="HA2016"></a> Hernandez, S., & Alvarez, A. (2019). Invernadero Capilla : Cultivos Bajo Cubierta. Retrieved 16 October 2019, from https://agroinvernaderos.webnode.es/tipos-de-invernaderos/invernadero-capilla/

1. <a name="IEP2019"></a> Invernaderos Túnel - IEP invernaderos. (2019). Retrieved 16 October 2019, from http://www.inverelpilar.com/es/invernaderos/invernaderos-tunel

1. <a name="ARD2019"></a> Arduino - Introduction. (2019). Retrieved 16 October 2019, from https://www.arduino.cc/en/guide/introduction
