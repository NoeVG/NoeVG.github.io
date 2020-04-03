---
title: |
  Control de Carrito Mediante Arduino y app Android
  ![](https://platform.togive.eu/assets/courseware/v1/4724af964716421484fb2b2bb290162f/asset-v1:ULL+TG-MOOC8-EN+2018-T1+type@asset+block/asset-v1-UAEMEX_TG-MOOC2-ES_2018-T1_type_asset_block_Logo_uaemex.png){width=50%}

author: Noé Vásquez Godínez
date: Marzo 24, 2020
toc: true # Añadir índice
lof: true # Añadir lista de figuras
lot: true # Añadir lista de tablas
lang: es


geometry:
- top=1in
- bottom=1in
- right=0.5in
- left=1.5in
mainfont: LiberationSans
fontsize: 12pt

layout: article

contenido:
  - section: Introducción
    link: introduccion

  - section: Objetivo
# build  pandoc carrito.markdown -o salida.pdf
---

# [Introducción](#introduccion)

Desarrollo e implementación del control de un carrito mediante la tarjeta de pruebas Arduino,
el control es remotamente mediante comunicación Bluetooth a través de una app Android.
El control del carrito es desde una aplicación Android
las ordenes de movimiento están determinados por los sensores de movimiento del smartphone Android.

En este documento se expone la construcción, armado y adaptación del carrito con Arduino,
así mismo el desarrollo de la aplicación android.

# Objetivo

Hacer uso de la tarjeta de pruebas Arduino, así mismo hacer aplicación
de los conocimientos de electrónica, programación y diseño de soluciones de software.

# Antecedentes de carritos de control

Trabajar con Arduino en algunos contextos nos relaciona a introducirnos a la robótica,
aunque cabe señalar que personas de la "vieja escuela" piensan que Arduino no se relaciona
con robótica, ya que para ellos robótica es desarrollar todo desde cero como son:
micro controladores, ensamblador, soldar, diseñar circuitos, estudio de paradigmas y una
alta formación en matemáticas y paradigmas de robótica; y en un determinado punto
tienen razón, por conectar (plug and play) sensores y tarjetas de control no nos
volvemos unos robotistas, sin embargo este tipo de proyectos o practicas
permiten tanto a un aficionado o estudiante adentrarse e interesarse por un estudio
más denso relacionado a la robótica, incluso la facilidad de implementación de tarjetas de pruebas
como Arduino permiten formase para el Internet de las cosas.

Continuando con el desarrollo de contenido atractivo para futuros lectores en esta sección
abordamos temas fundamentales e introductorios sobre robótica.

## Paradigmas de robótica

La palabra robot mantiene un origen en la obra de R.U.R (Rossum's Universal Robots), de Karel Čapek,
hace referencia a trabajos cansados y de alto desgaste (trabajos pesados).

Las funciones de un robot se pueden dividir entres categorías, la función de tomar informaciones de sensores
y realiza una salida con utilidad para otras funciones es nombrada **SENSE**, la función de la cual aparir de los datos
de sus sensores y del mundo exterior produce una o mas tareas relacionadas al movimiento o desempeño del robot es nombrada
**PLAN**, funciones que producen la salida de comandos es nombrada **ACT**.

## Navegación


# Materiales

| # | Material           | Descripcion |
| - | -------------------| -------------------------------|
| 1 | Arduino (UNO MEGA) | Puede ser el arduino básico, este se usara para el control de motores y comunicación Bluetooth|
| 1 | Sensor  Bluetooth  | Sensor hXX00 , para la comunicación Bluetooth |
| 1 | Driver L298        | Puente H para el control de motores|
| 1 | Jumpers Macho      | Conexiones |
| 1 | Jumpers Hembra     | Conexiones |
| 1 | Eliminador 12 VC   | Fuente de alimentación durante pruebas |
| 1 | Laminas pequeñas   | Adaptar el carrito e instalar piezas |
| 1 | Tornillos          | Asegurar los materiales |
| 1 | Interruptor        | Control de alimentación de VC|
| 1 | Pulsador           | Emitir sonidos de TEST y comunicación en el robot |
| 1 | Baterías           | Alimentación autónoma |
| 1 | Chasis de carrito eléctrico | Montaje de motores y arduino |


# Diagrama de Bloques

Se presenta el diagrama de bloques para el sistema

<img src="images/DiagramBloques.png" alt="Diagrama de Bloques" style="width:500px;height:600px;">

# Diagrama Eléctrico
## Conexion Bluetooth - Arduino
  En mi caso yo utilize el arduino Mega, pero en forma de guiá, se expone la siguiente
  conexión Bluetooth HC-06. El modulo Bluetooth HC-06 trabaja solo cliente muy distinto a su contra
  modulo el HC-05.

  En ambos módulos permiten la conexión  Bluetooth, esto permite
  la comunicación desde terminales Android o PC con módulos Bluetooth.

![Ejemplo salvado de: https://manualsupervivenciamaker.com](https://manualsupervivenciamaker.com/manual/images/MSM32_1.png){height=50% width=50%}

## Conexion Arduino motores
La conexión de los motores con Arduino se realizo mediante el Driver L298,
para que Arduino logre controlar los motores es necesario hacerlo mediante un puente H,
el puente H permite trabajar con la polaridad del motor para poder hacerlo girar
en diferentes direcciones (derecha/izquierda). La siguiente imagen expone
la conexión del driver L298:

![Ejemplo salvado de: https://forum.arduino.cc](https://forum.arduino.cc/index.php?action=dlattach;topic=598858.0;attach=295625){height=50% width=50%}

# Diagrama de flujo ( Arduino )

![Diagrama de Flujo Arduino](images/DiagramaArduinoCarrito.png ){height=50% width=50%}

# Diagrama de flujo ( App Android)

![Diagrama de Flujo Android](images/AndroidDiagrama.png ){height=50% width=50%}

# Construcción
En esta sección se presenta los momentos de construcción del carrito,
si usted esta desarrollando un proyecto similar quizás no deba replicar por completo
los siguientes pasos, pero si le pueden ser de utilidad para obtener ideas
al adaptar los materiales con los que usted cuente.

## Elementos físicos

### El chasis del carrito

El chasis,llantas y motores, se obtuvieron de un carrito de control remoto
su aplicación es para entretenimiento de niños (un juguete), este carrito se compro en
un Fleamarket en México a estos establecimientos se les llama Tianguis.

![Carrito inicial](images/carrito/IMG_20200211_134441.jpg ){height=40% width=40%}

![Carrito inicial](images/carrito/IMG_20200211_134616.jpg ){height=40% width=40%}

![Carrito inicial con su control remoto](images/carrito/IMG_20200211_134737.jpg ){height=40% width=40%}

![Deposito de baterías del carrito](images/carrito/IMG_20200211_134813.jpg ){height=40% width=40%}

![Deposito de baterías del carrito](images/carrito/IMG_20200211_134850.jpg ){height=40% width=40%}

Estas baterías no se usaran ya que no son recargables, y ademas seria un gasto innecesario junto
con una contaminación, quizás el deposito si se pueda usar para las baterías recargables.

![Deposito de baterías del carrito](images/carrito/IMG_20200211_134926.jpg ){height=40% width=40%}

![Deposito de baterías del carrito](images/carrito/IMG_20200211_135036.jpg ){height=40% width=40%}

### Modificación y adaptación del carrito

Debemos ver los motores e incluso desmontar el chasis de plastico, puesto que para el arduino
este puede estorbar.

![Abriendo el carrito](images/carrito/IMG_20200211_135318.jpg ){height=40% width=40%}

![Desmontando tornillos](images/carrito/IMG_20200211_135607.jpg ){height=40% width=40%}

![Desmontando carcase](images/carrito/IMG_20200211_135946.jpg ){height=40% width=40%}

![Desmontando carcase](images/carrito/IMG_20200211_135953.jpg ){height=40% width=40%}

![El carcase ya no se usara](images/carrito/IMG_20200211_140006.jpg ){height=40% width=40%}

Es necesario tener acceso a los motores, por debajo de esta tapa de plastico,
se debe encontrar los motores.

![Buscando motores](images/carrito/IMG_20200211_140110.jpg ){height=40% width=40%}

![Accesando a los motores](images/carrito/IMG_20200211_140547.jpg ){height=40% width=40%}

La placa de control de este carrito, no la vamos a utilizar, por ello esta la retiramos

![Accesando a los motores](images/carrito/IMG_20200211_140831.jpg ){height=40% width=40%}

![Accesando a los motores](images/carrito/IMG_20200211_141225.jpg ){height=40% width=40%}

![Retirando controladora](images/carrito/IMG_20200211_141549.jpg ){height=40% width=40%}

![Retirando controladora](images/carrito/IMG_20200211_141549.jpg ){height=40% width=40%}

![Retirando controladora](images/carrito/IMG_20200211_141908.jpg ){height=40% width=40%}

![Obteniendo motores](images/carrito/IMG_20200211_142031.jpg ){height=40% width=40%}

![Limpiando motores](images/carrito/IMG_20200211_143838.jpg ){height=40% width=40%}

### Instalación de componentes electrónicos
La placa Arduino esta instalada en el carrito, por ello es necesario definir como instalarlar y asegurarla

![La placa arduino y el carrito](images/carrito/IMG_20200211_144331.jpg ){height=40% width=40%}

Es necesario realizar mediciones y ajustes

![La placa arduino y el carrito](images/carrito/IMG_20200211_144952.jpg ){height=40% width=40%}


### Código Arduino
## App Android
### Desarrollo de la aplicación
### Codigo fuente Android

# Resultados



# Tabla de control(Fotos)
