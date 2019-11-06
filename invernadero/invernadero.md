
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
 style="width : 450px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de la imagen:
 <a href ="http://cabaseiot.com.ar" >http://cabaseiot.com.ar</a>
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
 style="width : 500px;"
class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de image: <a href="https://www.programoergosum.com">https://www.programoergosum.com</a>
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
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de image: <a href="https://www.arduinohobby.com/" >https://www.arduinohobby.com/</a>
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

Es una pequeña computadora, con un precio muy accesible para proyectos escolares o iniciales, esta mantiene puertos para conectarse tanto a un display dedicado o un monitor, las conexiones para teclado y mouse son mediante puerto USB, se puede instalar sistemas operativos GNU/Linux. El mayor provecho que se obtiene de Raspberry PI, es su posibilidad de interactuar con una gama alta de sensores, volviéndola muy atractiva para proyectos de electrónica [("Raspberry Pi Foundation - About Us", 2019)](#RAP2019).

### Características Raspberry PI

Cuando es necesario realizar actividades de automatización o de internet de las cosas con alto rendimiento, Raspberry PI se vuelve una opción muy atractiva, Raspberry PI cuenta con las siguientes características:

- Micro Ordenador o cumputadora SBC, de bajo costo

- Dimensiones pequeñas

- Microprocesador ARM con potencia de hasta 1 GHz

- Los primeros modelos con 512MB de Ran, actualmente ya tiene 1 Gb

- Incluyen una GPU Videocore IV

- Los Sistemas Operativos que se pueden instalar son: Raspbian, Arch Linux, RaspBMC, Pidora u OpenELEC, Windows 10.

### Lenguaje de programación

Los lenguajes de programación que esta soporta, están relacionados con el sistema operativo que se instale en la RaspBerry PI, al instalar sistemas GNU/Linux, prácticamente los lenguajes de programación más comunes pueden hacerse uso en la RaspBerry PI, tales como Java, JavasScript, C++, C, Python.

Siendo el lenguaje Python, el más empleado, tanto es el uso de Python en Raspberry Pi que ya se encuentran módulos en python para trabajar directamente con características propias de Raspberry Pi.

### Raspberry PI Hardware
Parte del hardware de raspberry PI es muy similar a las computadoras convencionales, sin embargo el puerto GPIO , es lo especial de Raspberry PI.

<center>
<img src="http://makermex.com/web/image/4340?access_token=0113bb6d-8f8b-44cf-ba0b-feb79ff6e04f"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de image: <a href="http://makermex.com">http://makermex.com</a>
</center>

El puerto General Purpose Input Output (GPIO), consta de pines que se pueden emplear como entradas y salidas de múltiple propósito, se encuentran en todas las Raspberry PI, pero con disposiciones diferentes.

<center>
<img src="http://makermex.com/web/image/4341?access_token=247aa22b-572f-41dd-b502-6f26f77b7525"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de image: <a href="http://makermex.com">http://makermex.com</a>
</center>

## Invernadero Inteligente

En las secciones anteriores, se exponen herramientas que permiten ser parte de soluciones para actividades que en la actualidad necesitan emplear recursos digitales e informáticos.

Una de las actividades en las que hacer uso de sensores, actuadores,  y tarjetas de uso general, es la implementación de Invernaderos Inteligentes.

En los invernaderos inteligentes se hace uso de dispositivos que estén automatizando actividades como es el riego y ventilación de un invernadero.

En un invernadero existen variables como la temperatura tanto del ambiente y del área próxima de los cultivos, así como la humedad de la tierra y del ambiente, que el conocerlas de forma precisa permitirá una optimización del invernadero.

### Propósito

Mediante el uso de sensores y actuadores, automatizar ciertas acciones en un invernadero, ciertas acciones pueden cubrir:

- Control climático

- Control de riego

- Control de temperatura

- Control de humedad

En otra parte toda la información que surge de estos controles,
se puede almacenar en una base de datos, para su posterior análisis,
esto con la finalidad aumentar el rendimiento de un invernadero.

## Invernadero caso practico

En el DIF (Sistema Nacional para el Desarrollo Integral
de la Familia) del Estado de México, se ha puesto en marcha la instalación de un invernadero, esta actividad esta bajo la supervisión del Ing. Crystian Pichardo González, jefe del departamento de
nutrición de esta misma institución.

En este invernadero, se desea controlar y automatizar ciertas actividades, es por ello que se es necesario realizar la planeación e implementación de recursos para volver este invernadero a uno inteligente.

### Ubicación del invernadero

El invernadero se encuentra con ubicación en Av.
Convento de Santa Mónica s/n , esq. Convento de San Fernando,
Fraccionamiento Jardines de Santa Mónica, Tlalnepantla de Baz,
Estado de México.
<center>
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1580.971886326558!2d-99.22559526049773!3d19.532766216886834!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85d21d2fa71d0325%3A0xc1d34267777fa1a0!2sDIF%20Tlanepantla!5e0!3m2!1sen!2smx!4v1571329249050!5m2!1sen!2smx" width="400" height="350" frameborder="0" style="border:0;" allowfullscreen=""></iframe>
</center>


<center>
<img src="http://www.tlalnepantla.gob.mx/img/noticias/4880.jpg"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Fuente de image: <a href="http://www.tlalnepantla.gob.mx">http://www.tlalnepantla.gob.mx</a>
</center>

### Especificaciones del invernadero

<center>
<img src="./img/photos/IMG_20190902_110102.jpg"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Primer plano del diseño del invernadero.
</center>

El invernadero estará trabajando con 4 parcelas, en estas parcelas se mantendrá el cultivo de rábanos, lechugas y cilantro.

<center>
<img src="./img/photos/IMG_20190902_095649.jpg"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Cultivo de Lechugas.
</center>
<br>
<br>
<center>
<img src="./img/photos/IMG_20190919_094441.jpg"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br>
 Invernadero.
</center>


En el siguiente plano se puede comprender con mas detalle las dimensiones del invernadero:

### Necesidades en este invernadero

En este invernadero se necesita controlar las siguientes variables:

- Control de humedad de tierra

- Control de temperatura de tierra

- Control de temperatura ambiente

En automatización se desea realizar lo siguiente:

- Control de riego

- Control de iluminación con bombillas.

Toda la información que se genere, es necesario recopilarla en una base de datos, para mostrar el historial y comportamiento de las variables como lo son temperatura y humedad, toda esta información debe visualizar de forma local en el invernadero y remotamente.

## Propuesta de Invernadero Inteligente

En cada parcela se instalaran sensores de humedad para tierra, así mismo sensores de humedad y temperatura ambiente, así mismo el riego para cada parcela estará controlado por electrovalvulas, la iluminación se realzara con bombillas, estos dos últimos estarán controlados mediante módulos relé, los cuales con pulsos electrónicos establecerán el encendido o apagado de cada uno.

<center>
<img src="./img/photos/diagramaSensoresGeneral.png"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diagrama general de parcelas y sensores.
</center>
<br>
Los sensores proporcionaran datos a las tarjetas Arduino, cada parcela estará dotada de una tarjeta Arduino, las cuales estarán controladas con un Arduino delegado como maestro, la comunicación entre los Arduinos (esclavos) con el Arduino (maestro) es mediante el protocolo conocido como I2C (Inter-integrated Circuit).

El envió de datos para su análisis se realizara mediante una tarjeta Raspberry PI, estos datos son obtenidos mediante la interfaz serial entre Raspberry PI y el Arduino maestro.

La visualización de estos datos se presentara en dos posibles formas:

- **Local:** Los datos se visualizaran directo en la Raspberry PI.

- **Remota:** Los datos se rescataran de la base de datos que la Raspberry PI estará alimentando, se empelara una aplicación WEB para poder mostrarlos.

El control de riego y la iluminación también estará disponible en la visualización de los datos.

<center>
<img src="./img/photos/diagramaSensoresGeneralArduinos.png"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diagrama general comunicación.
</center>
<br>

### Tarjetas
<center>

|Cantidad |Tarjeta | Aplicación |Imagen |
|:----------:|:--------:|:------------:|:------:|
| 4 | Arduinos | Esclavo, recopilación de datos desde sensores|<img src="https://www.steren.com.mx/media/catalog/product/cache/b69086f136192bea7a4d681a8eaf533d/a/r/ard-010_x1_12.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|
| 1 |Arduino | Maestro, lógica de operación.|<img src="https://www.steren.com.mx/media/catalog/product/cache/b69086f136192bea7a4d681a8eaf533d/a/r/ard-010_x1_12.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|
| 1 |RaspBerry PI | Envio de datos a base datos.|<img src="https://cdn-reichelt.de/bilder/web/xxl_ws/A300/RASP_03_01.png" style="width : 100px;" class="img-fluid img-thumbnail"/>|

</center>

### Sensores y otros

<center>

|Cantidad |Tarjeta | Aplicación |Imagen |
|:----------:|:--------:|:------------:|:------:|
| 12 | Sensor Humedad de Suelo | Se obtiene la huemdad del suelo mediante la resistencia en la tierra|<img src="https://images-na.ssl-images-amazon.com/images/I/31Z4onh5hyL.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|
| 13 |Sensor dht11 | Temperatura y humedad ambiente.|<img src="https://store.prometec.net/wp-content/uploads/2019/06/dht11.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|
| 3 |Electrovalvulas | Abren o cierrann el flujo de agua|<img src="https://images-na.ssl-images-amazon.com/images/I/41pAB6kBJEL._SX466_.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|
| 2 |Relé | Permite controlar dispositvos con AC o DC mayor de 5v |<img src="https://cdn-tienda.bricogeek.com/3535-thickbox_default/modulo-4-reles-5v.jpg" style="width : 100px;" class="img-fluid img-thumbnail"/>|

</center>

## Software

Se expone los lenguajes de programación a emplear relacionado a la construcción del software, así mismo se muestra la lógica de cada modulo mediante diagramas de flujo,
esto con la finalidad de comprender el funcionamiento en cada tarjeta, los lenguajes de programación dependen de la plataforma en las que se estará trabajando.

La plataforma Arduino se programa mediante el uso de un lenguaje propio basado en el lenguaje de programación de alto nivel Processing que es similar a C++, para RaspBerry PI se emplea Python, un lenguaje que contiene gran cantidad módulos ya listos para trabajar con especificaciones propias de Raspberry PI y como parte final para los DashBoard se empleara el Framework Angular para el Front-End  y Express para el Back-End, ambos propios de Nodejs, en el caso del DashBoard local se usara Python con QtPSyde2 para las tareas graficas.

### Programación en Arduino
Diagrama de flujo de datos para arduino maestro
<center>
<img src="./img/photos/diagramaMaestroArduino.png"
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diagrama de flujo para Arduino Maestro.
</center>
<br>
<br>
<center>
<img src="./img/photos/diagramaSlaveArduino.png "
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diagrama de flujo para Arduino Esclavo.
</center>
<br>
<br>

### Programación en Python
<center>
<img src="./img/photos/diagramaGeneralRasp.png "
 style="width : 500px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diagrama de flujo para RaspBerry PI.
</center>
<br>
<br>

### DashBoard web con Angular 8
<center>
<img src="./img/photos/diagramaDashboardAngular.png "
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
DashBoard online Angular
</center>
<br>
<br>

### DashBoard local con Python
<center>
<img src="./img/photos/diagramaDashboardPython.png "
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
DashBoard local Python QT
</center>
<br>
<br>

## Trabajando con sensores

### Simulación

La comunicación entre los arduino es mediante el protocolo i2c, este protocolo permite una comunicación bidireccional, permitiendo enviar y obtener datos desde el arduino maestro.

Por ello se presenta el codigo fuente sobre la implementación de i2c en arduino con 1 arduino maestro y 3 arduinos esclavos, esto con la finalidad de simular la parte fundamental de la comunicación entre los arduinos.

Datos de implementación:

|Arduino |Rol | Función |Datos enviar |Datos recibir |
|:----------:|:--------:|:------------:|:------:|:------:|
|Arduino 1 |Maestro|Controlar esclavos|Enviar a cada esclavo el codigo 1| Recibe de cada esclavo el valor de temperatura
|Arduino 2|Esclavo|Enviar datos a maestro|Enviar cada con temperatura valor 66 | orden de maestro
|Arduino 3|Esclavo|Enviar datos a maestro|Enviar cada con temperatura valor 77 | orden de maestro
|Arduino 4|Esclavo|Enviar datos a maestro|Enviar cada con temperatura valor 88 | orden de maestro

Código fuente maestro:

```
#include <Wire.h>
#define MESSAGE_LEN 32
#define ARDUINOS 3

void setup()
{
	Serial.begin(9600);  // Velocidad de conexión
}

void loop()
{
  //obtener informaciòn de todos.
  Wire.begin();        // Conexión al Bus I2C

  for(int i = 8; i <(8+ARDUINOS);i++){
    Serial.println("Working...");

    sendInformationSlave(i,1);
    delay(5000);
    getInformationSlave(i);           
  }
}
void getInformationSlave(int slave){
  Wire.requestFrom(slave, MESSAGE_LEN);    // Le pide 17 bytes al Esclavo 1
  int x = 0;
  char c[MESSAGE_LEN];
  while(Wire.available())    // slave may send less than requested
  {
    c[x++] = Wire.read();   // Recibe byte a byte
  }
  Serial.println("info");
  Serial.println(c);       // Cámbia de línea en el Serial Monitor.
}
// Esto es lo que envía cuando le hace la petición.
void sendInformationSlave(int slave,int code)
{
  Wire.beginTransmission(slave);
  Wire.write(code);
  Wire.endTransmission();
 //delay(5000);
}

// https://stackoverflow.com/questions/9072320/split-string-into-string-array
String getValue(String data, char separator, int index)
{
  int found = 0;
  int strIndex[] = {0, -1};
  int maxIndex = data.length()-1;

  for(int i=0; i<=maxIndex && found<=index; i++){
    if(data.charAt(i)==separator || i==maxIndex){
        found++;
        strIndex[0] = strIndex[1]+1;
        strIndex[1] = (i == maxIndex) ? i+1 : i;
    }
  }

  return found>index ? data.substring(strIndex[0], strIndex[1]) : "";
}
```

Código fuente esclavo 1 :
```
#include <Wire.h>
#define ID 8 // cambia para cada arduino
#define MESSAGE_LEN 32

char cadena[MESSAGE_LEN];

void setup() {
  Wire.begin(ID);      // join i2c bus (address optional for master)
  Serial.begin(9600);  // start serial for output
}

void loop() {  
  Serial.println("Get data from master");
  Wire.onReceive(reciveEvent);
  delay(1000);
  Wire.onRequest(enviarDatos);
  Serial.println("Finish send data");
}

void enviarDatos(void) {
  Wire.write(cadena);
}

void reciveEvent(int n) {
  String response;
  int x = Wire.read();

  switch (x) {
    case 1:

      //humedad
      Serial.print("Enviar Humedad Ambiente:");
      response = String("DatoHA,");
      response.concat("A_");
      response.concat(ID);
      response.concat(",");
      response.concat(66);
      response.concat(",");
      response.concat(66);
      response.concat(",");
      response.concat(66);
      response.concat(",");
      response.toCharArray(cadena, MESSAGE_LEN);
      Serial.println(cadena);
      break;
  }
  delay(5000);
  Serial.println("Finish recolected data from sensor");
}

```
<center>

Simulación en Tinkercad

<video width="600" controls>
  <source src="./videos/simulacioni2c.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
</video>
</center>


## Instalación

### Maestro y Esclavo

<center>
<img src="./img/photos/IMG_20190903_140847.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
 Diseño de envió de información
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20190903_140854.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Pruebas de comunicación
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20190903_140858.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Pruebas de comunicación
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20191003_101809.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Instalación en placa de soporte
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20190919_113157.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Fabricando placa de soporte
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20191003_101719_rotada.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Instalación en contenedor
</center>
<br>
<br>

<center>
<img src="./img/photos/IMG_20191003_141738_rotada.jpg"
 style="width : 600px;"
 class="img-fluid img-thumbnail"
 />
 <br><br>
Instalación Arduinos esclavos y maestro
</center>
<br>
<br>

### RaspBerry PI maestro

### Instalando Sensores

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

1. <a name="RAP2019"><a/> Raspberry Pi Foundation - About Us. (2019). Retrieved 16 October 2019, from https://www.raspberrypi.org/about/
