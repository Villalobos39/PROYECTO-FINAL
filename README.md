<p align="left">
  <img src="https://github.com/Villalobos39/PROYECTO-FINAL/blob/master/Imagenes/LOGO_TECNM_GRIS.png" width="350" title="hover text">
  <img src="https://github.com/Villalobos39/PROYECTO-FINAL/blob/master/Imagenes/sistemas%20computacionales.png" width="350" alt="accessibility text">
</p>

# PROYECTO-FINAL: Sistema Operativo Robótico

## ROS (Robot operating system).

Para poder sacar el máximo rendimiento a ROS, primero tenemos que comprender en qué consiste el sistema, y cuales son sus principales ventajas respecto al resto de sistemas que se pueden encontrar hoy en día. Un robot es una máquina controlada por ordenador y programada para moverse, manipular objetos y realizar trabajos a la vez que interacciona con su entorno.

#### Los robots exhiben tres elementos claves según la deﬁnición adoptada

○ Programable, lo que signiﬁca disponer de capacidades computacionales y de manipulación de símbolos (el robot es un computador). 

○ Capacidad mecánica, que lo capacita para realizar acciones en su entorno y no ! ser un mero procesador de datos (el robot es una máquina).

○ Flexibilidad, puesto que el robot puede operar según un amplio rango de ! programas y manipular material de formas distintas.

![ERROR FATAL jiji](https://github.com/Villalobos39/PROYECTO-FINAL/blob/master/Imagenes/Rbot.png)

### ¿ Qué es ROS ?

Es similar a otras plataformas de desarrollo para robots existentes en la actualidad, y su mayor virtud, es la de haber sabido aunar lo mejor de cada uno de estos sistema, juntando todo en un solo sistema capaz de comunicarse tanto con los robots mas modernos, como con los ya existentes en el mercado. Desde su creación, ROS se ha diseñado para facilitar el intercambio de software entre los aﬁcionados y los profesionales de la robótica en todo el mundo debido a su enfoque didáctico y abierto, lo que ha permitido la construcción de una gran comunidad de colaboradores a lo largo de todo el mundo. 

![ERROR FATAL jiji](https://github.com/Villalobos39/PROYECTO-FINAL/blob/master/Imagenes/ROS.jpg)

### El objetivo de ROS
El objetivo de ROS no es ser un sistema pionero en la robótica, el objetivo principal de ROS es apoyar el código reutilizable en la investigación robótica y el desarrollo. 
El sistema es una estructura distribuida en procesos que permite a los ejecutables ser diseñados de forma individual y utilizarse de forma ﬂexible en tiempo real.

○ Sencillez: ROS está diseñado para ser tan sencillo como sea posible de modo que el código escrito para ROS se pueda utilizar con otros marcos robot de software. 

○ ROS es fácil de integrar con otros sistemas operativos de robots y ya ha sido integrado con OpenRAVE, Orocos y Player. 

○ Modelo de bibliotecas: es el modelo de desarrollo preferido, consiste en escribir una serie de programas con interfaces funcionales y limpias que permitan una rápida modiﬁcación. 

○ Independencia de idiomas: el marco ROS es fácil de implementar en cualquier lenguaje de programación moderno. Se ha implementado en Python, C++, y LISP; y actualmente existen  bibliotecas experimentales en Java y Lua.

○ Modo test: ROS tiene una orden llamada ROSTEST que hace que sea fácil acceder a un modo prueba de sistema. 

○ Escala: ROS es adecuada para sistemas grandes y ejecución de los procesos de gran tamaño.



### Compatibilidad con los sistemas operativos 
ROS también es compatible con el sistema de repositorios, que permiten la colaboración a nivel internacional permitiendo tomar decisiones independientes sobre el desarrollo y la ejecución, pero con la ventaja de poder ayudarse de las herramientas o archivos creados por otros en sus proyectos.

@@ -63,10 +71,51 @@ Son recursos que se encuentran en el propio programa:
![ERROR FATAL jiji](https://github.com/Villalobos39/PROYECTO-FINAL/blob/master/Imagenes/sistema-de-archivos-esquema.jpg)

### Computación a nivel Gráﬁco. 
La computación a nivel gráﬁco es la red ROS que se encarga de procesar todos los datos. Un sistema de control de robot comprenderá usualmente muchos nodos.
La computación a nivel gráﬁco es la red ROS que se encarga de procesar todos los datos. Los conceptos básicos son nodos , maestro , mensajes y temas,  los cuales proporcionan los datos de diferentes maneras: 

○ Nodos: Los nodos son procesos que llevan a cabo cálculos. ROS está diseñado para ser modular en una escala básica. Un sistema de control de robot comprenderá usualmente muchos nodos. 

○ Maestro: El Maestro proporciona registro de nombres y la búsqueda para el resto de la Computación Gráﬁca. Sin el Maestro, los nodos no serían capaces de encontrar mensajes entre sí, intercambiar, o invocar los servicios.

○ Mensajes: Los nodos se comunican entre sí pasando mensajes. Un mensaje es simplemente una estructura de datos que comprende los tipos de campos.

○ Temas : Los mensajes se enrutan a través de un sistema de transporte de publicación / suscripción semántica. Un nodo envía un mensaje por publicar a un determinado tema. El tema es un nombre que se utiliza para identiﬁcar el contenido del mensaje.

### La comunidad y ROS
Los conceptos comunitarios ROS Nivel ROS son recursos que permiten a las comunidades el intercambio del software y del conocimiento. Estos recursos incluyen:

○ Distribución: Son colecciones de versionadas en pilas que se pueden instalar. Las distribuciones juegan un papel similar al de las distribuciones de Linux.

○ Repositorios: ROS se basa en una red federada de repositorios de código, donde diferentes instituciones pueden desarrollar y lanzar sus propios componentes de software del robot. 

○ El wiki de ROS6: La comunidad Wiki es el foro principal para documentar la información sobre ROS. Cualquier persona puede inscribirse con una cuenta y contribuir con su propia documentación, facilitar las correcciones o actualizaciones, escribir tutoriales y más.

○ Respuestas de ROS: un sitio de preguntas y respuestas para contestar a las preguntas relacionadas con ROS. 

○ Blog: El blog de Willow Garage(creador de ROS) ofrece actualizaciones periódicas, incluyendo fotos y videos.

### Instalación del sistema
Vamos a comenzar con la toma de contacto con el programa, y para ello vamos a enumerar los pasos necesarios para poder usarlo en algunos de los sistemas operativos soportados, aunque en nuestro caso se detalla más Ubuntu ya que es con el que se ha realizado este documento.

#### a.Sistema Linux
Primero comprobamos que tengamos actualizado nuestro sistema, en esta versión podemos encontrar en la parte izquierda de la pantalla principal el programa llamado “update manager”.

a. Para comenzar abrimos la utilidad de Terminal. 

b. A continuación preparamos el sistema para que acepte los paquetes de información de la página del repositorio packages.ros.org, para ello usamos la función correspondiente a nuestro sistema.

**$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu precise main" > /etc/apt/ sources.list.d/ros-latest.list'**

c. Tras introducir la función anterior, nos pedirá la contraseña de usuario para conﬁrmar que queremos aceptar esta función, y terminal volverá a modo espera.

d. Lo siguiente es descargarte el ﬁchero correspondiente a tu teclado, para ello usamos la función:

**$ wget http://packages.ros.org/ros.key -O - | sudo apt-key add**

Por ejemplo, un nodo controla un telémetro láser, un nodo controla los motores de las ruedas, un nodo realiza localización, un nodo realiza la planiﬁcación de ruta, un nodo proporciona una vista gráﬁca del sistema, y así sucesivamente. Sin el Maestro, los nodos no serían capaces de encontrar mensajes entre sí, intercambiar, o invocar los servicios. Un mensaje es simplemente una estructura de datos que comprende los tipos de campos. Los mensajes pueden incluir estructuras arbitrariamente anidadas y matrices .
Una vez preparado nuestro sistema para instalar ROS procedemos a la instalación del sistema operativo, para ello usamos la función que nos descargara el sistema por completo (en el caso de tener algún tipo de problema con la instalación de alguna fase se puede instalar uno por uno todos los componentes necesarios).

Un nodo envía un mensaje por publicar a un determinado tema. Un nodo que está interesado en un determinado tipo de datos se suscribe al tema correspondiente. Puede haber varios editores y suscriptores concurrentes a un mismo tema, y un único nodo puede publicar y / o suscribirse a múltiples temas. La comunidad y ROS.
e. Primero comprobamos que esté todo actualizado con la función:
**$ sudo apt-get update**

Los conceptos comunitarios ROS Nivel ROS son recursos que permiten a las comunidades el intercambio del software y del conocimiento.
f.Luego usamos la función:
**$ sudo apt-get install ros-groovy-desktop-full**
