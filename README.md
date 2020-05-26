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

Y nada más pulsar la tecla intro el programa se pondrá a funcionar descargando todo lo necesario para que el sistema funcione.
Durante la instalación podremos conﬁgurar varios aspectos que tendrá nuestro sistema, como por ejemplo si solo va a trabajar en modo local, o se podrá utilizar también en remoto.

g. Cuando termine de descargar e instalar todos los paquetes deberemos ver algo parecido a esto:

h. A continuación iniciamos el programa rosdep y comprobamos que esté actualizado, para ello usamos primero la función: **$ sudo rosdep init**

i. Luego la función:  **$ rosdep update**

Ya tenemos ROS instalado en nuestro sistema Ubuntu, y ahora solo nos quedaría añadir un par de configuraciones más que son recomendables.

j. La primera es para que las variables de entorno que creemos se añadan automáticamente a nuestra sesión, para ello usamos la función:
**$ echo “source /opt/ros/groovy/setup.bash” >> ~/.bashrc**

Luego: 
**$ source ~/.bashrc**

k. También es conveniente instalar rosinstall, que es un añadido que nos permitirá descargarnos fácilmente el código fuente de muchos añadidos con solo un comando, para ello usamos el comando: 
**$ sudo apt-get install python-rosinstall**

l. Tras esto ya tendremos nuestro sistema listo para trabajar con el.

#### b. Sistemas MAC OS X
Para proceder a instalar ROS en MAC OS X, primero deberemos descargarnos un programa denominado Homebrew que nos permitirá y ayudará a instalar todo lo necesario para poder trabajar con él.

La aplicación homebrew se instala escribiendo en el terminal de MAC OS X el siguiente código:
**ruby -e “$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)”**

tras indicarle al programa que estamos seguros que queremos instalar el programa, se descargara e instalara todo los componentes del programa De forma adicional podemos ejecutar desde terminal el código:
**brew doctor** 

El programa comprobará los archivos que va a necesitar, si están instalados o desactualizados. 
Lo siguiente que debemos hacer es instalar el software adicional necesario:
**$ brew update 
$ brew install cmake**

Ahora comenzamos a descargar los primeros ﬁcheros necesarios para ROS, en este caso la distribución Hydro.
**$ brew tap ros/hydro 
$ brew tap Homebrew/science**

Ahora necesitaremos añadir a nuestro ﬁchero /.bashrc lo necesario para que hombrew trabaje de forma conjunta con terminal: 
**export PATH=/usr/local/bin:/usr/local/share/python:$PATH**
export PYTHONPATH=” /usr/local/python2.7 /site-packages:$PYTHONPATH” 

Ahora conﬁguramos el terminal para que cada vez que lo abramos no tengamos que introducir esta última parte del código:
**$ brew untap ros/DISTRO**

Ahora prepararemos nuestro sistema para poder descargar los ultimos ﬁcheros necesarios para usar ROS:
**$ sudo easy_install pip
$ sudo pip install -U wstool rosdep rosinstall rosinstall_generator rospkg catkin-pkg Distribute 
$ sudo rosdep init 
$ rosdep update**

Ahora vamos a crear un espacio de trabajo para catkin. 
**$ mkdir ~/ros_catkin_ws 
$ cd ~/ros_catkin_ws**

Ahora vamos a instalar las librerías o complementos necesarios para ROS:
**$ rosinstall_generator desktop-full --rosdistro hydro --deps --wer-only > hydro-desktop-fullwet.rosinstall
$ wstool init -j8 src hydro-desktop-wet.rosinstall**

También podemos descargar lo básico para el uso usando los dos códigos anteriores, pero solo poniendo desktop en lugar de desktop-full. Ahora procedemos a comprobar que tenemos todas las dependencias requeridas:
**$ rosdep install --from-paths src --ignore-src --rosdistro hydro -y**

Así ya tendremos nuestro sistema preparado para poder usar ROS.

#### c. Sistemas Windows
Este es posiblemente el más sencillo de todos los sistemas para instalar ROS, aunque no se debe olvidar que los ﬁcheros para trabajar con Windows están en fase Beta, y no están exentos de fallos de programación, y desde la propia página de Willow Garage nos invitan  a ayudar a mejorarlo.
Para proceder a la instalación solo deberemos ir a la página:
 http://wiki.ros.org/win_ros/hydro/Msvc%20SDK 
descargarnos y ejecutar los ﬁcheros necesarios para su correcto funcionamiento.

### Primeros pasos con ROS

#### 1. Iniciar/configurar el programa
Una vez que tenemos el sistema en nuestro ordenador, vamos a proceder a mostrar el funcionamiento básico de ROS para más adelante poder comprender más a fondo el sistema a nivel jerárquico.
En este caso para probar que la configuración del programa sea la correcta vamos a utilizar uno de los programas ya creados y que podemos encontrar dentro de la página de ROS, hablamos de turtlesim, que es un sencillo programa que utilizaremos de aquí en adelante para nuestro ejemplo.

a. Para descargarnos esta distribución a nuestro sistema utilizaremos el comando: **$ sudo apt-get install ros-fuerte-ros-tutorials**

b. Después de introducir nuestra contraseña de administrador nos debería aparecer una pantalla como esta:

c. Cuando llegue al 100% terminal volverá al modo de espera y ya tendremos instalado nuestro ejemplo.

#### 2. Ejecutar un programa
a. Para ejecutar nuestro programa de prueba tendremos que abrir una nueva ventana de terminal y teclear: **$ rosmake turtlesim**

b. Luego del que el programa nos generará todo el directorio turtlesim con todo lo necesario para trabajar con él.

También señalar que este paso solo es necesario la primera vez que ejecutamos el programa, las demás veces podremos obviar este paso, ya que en nuestro sistema ya tendremos todos los ﬁcheros generados y solo habrá que activarlos.

c. Después solo tendremos que teclear **$ rosrun turtlesim turtlesim_node**

d. Finalmente con esto veremos algo parecido a esto:

#### 3. Ejecutar un subprograma
Ahora vamos a proceder a interactuar con nuestro programa, para ello vamos a activar un subprograma que nos va a permitir manejar con el teclado la tortuga que vemos en nuestra pantalla.

a. Para ello abrimos una nueva ventana de terminal e introducimos: **$ rosrun turtlesim turtle_teleop_key**

b. Ahora ya puedes mover con las teclas de dirección la tortuga del ejemplo.

### ROS en profundidad
Tras una breve explicación vamos a proceder a una explicación más en profundidad de cómo funciona ROS, su jerarquía y su forma de trabajar.

#### Estructura
Lo primero que vamos a ver es la estructura del sistema operativo, de lo más global (repositorio) a lo mas especiﬁco (nodo).

#### Repositorio
Son ﬁcheros compuestos por uno o más paquetes y pilas, y que nos permiten descargarnos los ﬁcheros necesarios de forma más cómoda.

#### Pila (Stack)
Es una colección de paquetes que comparten una misma funcionalidad, sería el equivalente a una librería en otros sistemas de programación, y dentro de estos podemos encontrar unos ﬁcheros con metadatos que nos proporcionan la información para que estos funcionen de forma correcta (dependencias, compilación...).

#### Paquete
Es la unidad principal de organización en ROS, contiene todo lo necesario para hacer ser funcional y es análogo a un paquete en C.

#### Nodo
Son los procesos ejecutable que están incluidos dentro de los paquetes. Normalmente se utilizan varios nodos en los programas.

### Computación en ROS

#### a. Servicios
Es el tipo de arquitectura encargada de realizar la comunicación entre nodos, utilizan dos tipos de mensajes, uno para la solicitud, y otro que es la respuesta dada por el otro nodo a esa petición. En los programas podremos encontrar nodos servidor y nodos clientes. Tras realizar la solicitud, el nodo servidor se queda en modo espera hasta recibir respuesta por parte del nodo cliente, y en el caso de que sea el cliente el que realiza una petición, el nodo servidor la procesa y responderá al cliente con la información requerida.

#### b. Tópicos
Tópicos o temas, son los nombres que identiﬁcan el contenido de un mensaje; y estos se enrutan de dos formas, una publicador y otra suscriptor. Un nodo que está interesado en un determinado tipo de datos se suscribe al tema correspondiente. 
Puede haber varios editores y suscriptores concurrentes a un mismo tema, y un único nodo puede publicar y / o suscribirse a múltiples temas.  En general, los editores y suscriptores no son conscientes de la existencia de los demás. 

#### c. Mensajes
Los nodos se comunican entre sí pasando mensajes. Un mensaje es simplemente una estructura de datos, que comprende los tipos de campos.

#### d. Maestro
El Maestro proporciona registro de nombres y la búsqueda para el resto de los nodos. Sin el Maestro, estos no serían capaces de encontrar mensajes entre sí, intercambiar, o invocar los servicios, lo que hace que sea totalmente indispensable a la hora de ejecutar cualquier tipo de programa.

#### e. Bags
Las bolsas son un formato para guardar y reproducir datos de un mensaje de ROS, permitiéndonos almacenar una serie de órdenes y después repetirlas secuencialmente.





