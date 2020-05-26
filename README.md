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

### El desarrollo de un programa

#### a. Espacio de trabajo
Como en cualquier otro programa, en nuestro sistema necesitaremos un lugar donde trabajar, en este caso se requiere de un área para crear nuestras pilas y paquetes, y su posterior modificación en caso de ser necesario. Para crear un nuevo espacio de trabajo utilizaremos el comando rosws, que se utiliza de la forma: 
          **$ rosws init [nombre del espacio de trabajo] [localización de los ﬁcheros de ros]**
          
Por ejemplo, para crear un espacio de trabajo llamado prueba UPCT lo haremos de la forma: 
          **$ rosws init prueba UPCT  /opt/ros/fuerte**
          
Al ejecutar este comando, automáticamente se crearán una serie de archivos necesarios dentro de una carpeta localizada en home/nombre_de_usuario/prueba UPCT, en este caso nos creará setup.bash, setup.sh, setup.zsh además de un archivo oculto denominado .rosinstall dentro de esta carpeta.

### Sistema de archivos
Utilizando el comando rosws visto en el punto anterior, todos los paquetes serán incluidos de forma automática dentro de la variable ROS_PACKAGE_PATH cada vez que llamamos al archivo setup.bash del espacio de trabajo necesario. Por ejemplo, para poder crear una subcarpeta dentro de nuestro espacio de trabajo, utilizaremos la función mkdir y añadiremos la carpeta paquete prueba, y esto se haría de la siguiente forma:
                      **$ mkdir prueba UPCT/paquete prueba**

A continuación lo que haremos es seleccionar nuestro espacio de trabajo, para que de forma automática todos los paquetes se incluyen en el directorio anterior. 
                      **$ rosws set home/Nombre_de_usuario/prueba UPCT/paquete prueba 
                      $ source /prueba UPCT/setup.bash**
                      
Si queremos también se puede configurar el programa para dejar configurado el entorno de forma automática para cada vez que se abra un nuevo terminal, para ello utilizaremos las siguientes funciones:

**$ echo"source/opt/ros/fuerte/setup.bash">>~/.bashrc 
$ echo"exportROS_PACKAGE_PATH=~/miworkspace:$ROS_PACKAGE_PATH">> ~/.bashrc 
$ echo"exportROS_WORKSPACE=~/miworkspace">>~/.bashrc 
$ echo"exportROS_HOSTNAME=localhost">>~/.bashrc 
$ echo"exportROS_MASTER_URI=http://localhost:11311">>~/.bashrc**

#### a. Packages y Stacks
Los Packages y los Stacks son los que anteriormente denominamos paquetes y pilas, pero le hemos dejado su nombre original para una mayor facilidad a la hora de familiarizarnos en esta parte del documento. Para ir a una ubicación especíﬁca dentro de un package o stack usaremos la función roscd, que se usa de la forma:
**$ roscd Localizacion_del_ﬁchero**

Si utilizamos esta función sin argumentos, nos llevará directamente al espacio de trabajo Para ver una lista con los ﬁcheros contenidos dentro de un package o stack tecleamos el código rosls:
**$ rosls Localizacion_del_ﬁchero**

Para esta última función existe una pequeña herramienta ya incorporada que nos ayudará en nuestro trabajo, ya que podemos empezar a escribir el nombre de los paquetes o las pilas y cuando tengamos más de dos letras escritas, si pulsamos la tecla tabulador, él nos completará el nombre de forma automática.

#### b. Rospack
Rospack es una herramienta que sirve para recuperar información en los paquetes de ROS, de forma parecida a como se haría bajo el entorno Linux con los comandos cd o ls. Podemos encontrar una amplia variedad de comandos que van desde la localización de paquetes de ROS en el sistema de archivos, a un listado de pilas disponibles. Una función que nos puede ayudar mucho sería:  
**$ rospack help**

Donde nos mostrará todos lo comandos disponibles bajo esta función. Un ejemplo de uno de los comandos disponibles sería, en el caso de querer encontrar un paquete, y se utilizaría de la forma: 
**$ rospack ﬁnd Nombre_del_paquete**

#### c. Rosstack
Rosstack es una herramienta de línea de comandos que nos permite recuperar información sobre las pilas en ROS. Implementa una amplia variedad de comandos que van desde la localización de las pilas de ROS en el sistema de archivos, a la lista de pilas disponibles para el cálculo del árbol de dependencia de las pilas.También se utiliza en ROS para el cálculo de la información y para construir las pilas. Su uso es muy parecido al descrito en el apartado anterior con los packages, solo habría que sustituir pack por stack, es decir usar el comando:  **$ rosstack**

### Motor de ejecución
El motor de ejecución es una colección de nodos y programas básicos necesarios para poder trabajar con ROS, y es esencial para que todos los nodos se puedan comunicar entre sí. 
Entre los nodos y programas básicos que se inician con el motor de ejecución podemos encontrar el master, el servidor de parámetros y el nodo rosout que es el encargado de trabajar con toda la información del registro de ROS. Este motor de ejecuta abriendo un terminal exclusivamente para él e introduciendo: 
**$ roscore**
Una vez introducido dicho comando, deberíamos ver algo parecido a esto:

### Obtener datos

#### a. Nodos
Un nodo es como si fuera un ejecutable dentro del paquete de ROS, usa la librería cliente de ROS para comunicarse con otros nodos, y estos pueden publicar o subscribirse a un tópico, además de usar cualquier servicio. ROS nos permitirá usar nodos creados con otros lenguajes de programación (phyton y c+ +) Para poder acceder, modiﬁcar y crear cualquier nodo necesitaremos los paquetes: roscode, rosnode y rosrun.
El primer paso será activar roscore tal y como hemos visto en el punto anterior. Justo después activaremos nuestro programa de prueba turtle y el nodo teleop turtle para poder ver su funcionamiento. Ahora vamos a veriﬁcar qué nodos están activos, para ello utilizaremos rosnode, introduciendo en el terminal: 
**$ rosnode list**

y se debería ver una respuesta:

Esto signiﬁca que en este caso está activo el nodo “rosout” (es un nodo que siempre tiene que estar activo, y es el encargado de recoger y registrar todos los nodos de depuración), y los nodos turtlesim (nos muestra la tortuga por pantalla) y teleop turtle (encargada de mover la tortuga cuando pulsamos las teclas de dirección de nuestro equipo).

#### b. Tópicos
Los tópicos, o también llamados temas, es el sistema usado por los nodos para comunicarse entre ellos. Lo primero que debemos hacer para poder comprender los tópicos, es activar los nodos que queramos usar, para ello usamos la función del apartado anterior: 
**$ rosrun [nombre_paquete] [nombre_nodo]**

Por facilidad de comprensión y usabilidad, al igual que en los ejemplos anteriores, vamos a hacer uso de los archivos de prueba llamados turtlesim, y turtle teleop.  Ahora podremos usar las ﬂechas del teclado para describir una trayectoria (en caso que no puedas usar las ﬂechas para dirigirla, prueba a tener activa la pantalla de terminal correspondiente al nodo turtle_teleop_key). 
Para poder ver más a fondo su funcionamiento, usaremos el paquete rqt_graph, cuya función es la de crear gráﬁcos dinámicos del sistema sobre lo que va a suceder en tiempo real. Para asegurarnos de que tenemos este paquete instalado usamos la siguiente función de terminal: 
**$ sudo apt-get install ros -<distribucion-usada>-rqt**
  
Sustituyendo distribucion-usada, por tu distribución de ROS (Fuerte, Groovy, etc.)  Una vez veriﬁcado, o en su caso instalado el paquete, procedemos a usarlo, tecleando en un nuevo terminal: 
**$ rosrun rqt_graph rqt_graph**

El programa debería mostrar una pantalla parecida a la siguiente:

Si pasas el cursor por encima de turtle1/command_velocity/ te mostrará en diversos colores los nodos y los tópicos de los que hace uso. Tal y como se puede observar, los nodos /turtlesim y /teleop_turtle, se comunican mediante el tópico turtle1/ command_velocity/

El comando rostopic nos proporciona información acerca de los tópicos, y podemos acceder a las diferentes opciones que nos ofrece esta función con el comando: 
**$ rostopic -h**

Donde nos mostrará la ayuda de esta función:

#### c. Mensajes
Un mensaje es una estructura de datos simples que sirven para que los nodos se comuniquen entre sí. 
Los mensajes soportan la mayoría de estructuras de datos usados en la actualidad (enteros, decimales, booleanos, etc.), así como las estructuras anidadas. 
Los mensajes son guardados en un ﬁchero msg en un subdirectorio del paquete, y usan el nombre estándar de ROS, por ejemplo:
 **std_msgs/msg/string.msg;**
 
Como medida de seguridad adicional, los mensajes usan MD5, lo que nos permite saber en todo momento si hay alguna parte del mensaje o del nodo que no esté funcionando correctamente, esto nos permite por ejemplo que cuando un nodo se comunica con otro mediante un mensaje, si este está incompleto, el sistema lo puede detectar al momento y no tener en cuenta este mensaje, realizando una petición de que se vuelva a enviar. 
Un mensaje puede incluir un tipo especial de mensaje llamado encabezamiento, que incluye algunos metadatos comunes para este tipo de ﬁcheros (número de identiﬁcación, marcas de tiempo, etc.).

#### d. Servicio
Los servicios son los encargados de permitir que los nodos envíen peticiones y reciban respuestas. 
Tal y como sucede con los tópicos, aquí disponemos de diversas funciones que nos pueden ayudar a comprender y actuar con nuestro sistema. 
El comando para acceder a estas funciones funciona de la forma: 
**$ rosservice [argumento]**

Los diferentes argumentos que existen para esta función son: 
**-list** 

Muestra la información acerca de un servicio activo. 
**-call** 

Llama a un servicio con los argumentos seleccionados, por ejemplo para vaciar un servicio, utilizaremos el argumento clear, lo que hará que se borren todos los datos introducidos con anterioridad. 
**$ rosservice call clear
 -type**
 
Imprime un servicio. 
**-ﬁnd**

Encuentra servicios. 

### Sistema de depuración
Dentro de ROS podemos encontrar un sistema de depuración mediante el cual podemos ver el funcionamiento de cada uno de los nodos y sus interacciones con otros para poder comprobar que el programa se comporte de la forma esperada. Para activar dicho sistema utilizaremos el código: 
**$ rqt_console**

### Trabajar con datos
Para trabajar con los datos que nos devuelve el programa mediante sus nodos, utilizaremos la función rosbag, lo primero que vamos a ver es como guardar estos datos para poder procesarlos en el momento que queramos. 
**$ mkdir bagﬁles**  // esto nos genera un directorio denominado bagﬁles en nuestro sistema. 
**$ cd bagﬁles**  //accedemos a la carpeta bagﬁles. 
**$ rosbag record -a**  //comenzamos la grabación de datos.

Podemos probarlo con nuestro programa de prueba de la tortuga que hemos utilizado en el apartado de primeros pasos con ROS, para ello primero inicializamos el programa, y probamos a mover la tortuga, tras varios movimientos podemos cerrar la aplicación rosbag y ver el archivo generado (el ﬁchero lo podemos encontrar dentro de nuestra carpeta /home/bagﬁles, y como nombre tendrá la fecha y hora de creación del ﬁchero).

Para visualizar los datos guardados, solo tendremos que usar la función: 
**$ rosbag info Nombre_del_ﬁchero**

En nuestro caso quedaría: 
**$ rosbag info 2013-09-06-19-10-47.bag**

Para volver a recuperar los datos guardados, para que el programa siga por donde se quedó solo tenemos que añadir play tras el comando rosbag:
**$ rosbag play Nombre_del_ﬁchero**

Que en nuestro ejemplo sería así: 
**$ rosbag play 2013-09-06-19-10-47.bag**

### Visualizando los datos
ROS tiene una función que nos puede ayudar mucho a la hora de saber como trabaja nuestro sistema, y de si lo está haciendo de forma correcta, esta función es rqt_graph, y nos mostrará de forma gráﬁca los nodos que están en funcionamiento, sus dependencias y su forma de trabajar. 
Para utilizar esta función solo tenemos que introducir en un terminal nuevo la función
 **$ rqt_graph**
En la imagen que podemos ver a continuación podemos ver un ejemplo de su funcionamiento con el programa turtle.

### Virtualizando ROS

#### a. Rviz
ROS dispone de una herramienta de visualización en 3D llamada RVIZ que posibilita que nuestro robot Qbo, o prácticamente cualquier otra plataforma robótica, pueda ser representada en imagen 3D, respondiendo en tiempo real a lo que le ocurre en el mundo real. 
RVIZ se puede usar para mostrar lecturas de sensores, datos devueltos por la visión estereoscópica (Cloud Point), hacer SLAM (localización y mapeo simultáneo) evitando obstáculos, etc. 

En el caso de robots con muchas articulaciones ROS dispone de otra herramienta llamada TF que es una biblioteca que facilita la elaboración en estos casos. De todas formas ROS tiene modelos ya creados para probar con RVIZ:

Lo primero que tenemos que hacer es inicializar ROS, abriendo una ventana desde la terminal y escribiendo en ella: 
**$ roscore**

Luego abrimos otra ventana desde terminal y escribimos: 
**$ rosrun rviz rviz**

Cuando terminemos de trabajar con el programa, para cerrarlo simplemente tendremos que ir a la ventana de terminal donde lo activamos y pulsar la combinación de teclas Ctrl + C.

#### b. Gazebo
Gazebo es un simulador gráﬁco de código abierto que se integra perfectamente con ROS y nos permite virtualizar nuestro robot, así como el entorno sobre el que va a funcionar, permitiéndonos probar el funcionamiento de este en un entorno controlado antes de llevarlo a la realidad, ayudándonos a ahorrar dinero y esfuerzos a la hora de crear un sistema desde cero o utilizar un sistema ya generado con anterioridad. Primero procedemos a instalarlo en nuestro sistema. 
**$ sudo apt-get install ros-groovy-simulator-gazebo**

Ahora procedemos a instalar el robot de prueba 
**$ sudo apt-get install ros-groovy-pr2-simulator**

Tenemos multitud de opciones a la hora de utilizar Gazebo, en este caso vamos a inicializar el programa con un mundo virtual vacío sobre el que pondremos un robot de ejemplo creado por los programadores de ROS (Willow Garage), para ello abrimos una ventana de terminal y ponemos la función: 
**$ roslaunch gazebo_worlds empty_world.launch**

Esto nos abrirá una ventana parecida a esta.

Ahora vamos a añadir el robot citado anteriormente, en este caso el robot PR2
**$ rosmake pr2_gazebo 
$ roslaunch pr2_gazebo pr2.launch**

Una vez que tengamos el robot en nuestro mundo virtual, ya podremos utilizarlo como si estuviéramos en la vida real, o bien mediante nodos automatizados, o bien añadiendo nodos que nos permitan moverlo de forma manual.Y ahora vamos a añadir el robot citado anteriormente, en este caso el robot PR2:
**$ rosmake pr2_gazebo 
$ roslaunch pr2_gazebo pr2.launch**

Una vez que tengamos el robot en nuestro mundo virtual, ya podremos utilizarlo como si estuviéramos en la vida real, o bien mediante nodos automatizados, o bien añadiendo nodos que nos permitan moverlo de forma manual.
Cuando terminemos de trabajar con el programa, para cerrarlo simplemente tendremos que ir a la ventana de terminal donde lo activamos y pulsar la combinación de teclas Ctrl + C.

### Aplicación

#### a. Creando nuestra aplicación
Ahora que ya conocemos el sistema de ROS en profundidad vamos a proceder a crear nuestro propio programa, y que mejor para mostrar su funcionamiento que crear el primer programa típico en todos los sistemas, el denominado “Hola Mundo”, para ello vamos a generar nuestro espacio de trabajo.  El paquete que contendrá nuestro programa y un nodo que muestre por pantalla esta frase.

#### b. Preparando el sistema
Lo  primero que vamos a hacer es crear nuestro espacio de trabajo, esto nos permitirá tener un lugar donde guardar nuestro programa y poder trabajar tanto con el que vamos a crear ahora como con proyectos personales futuros. 
Vamos a crear nuestro espacio de trabajo, indicando a nuestro sistema que genere todo lo necesario para utilizarlo como un paquete de ROS, al igual que lo tiene en el directorio opt/ROS:
**rosws init ~/groovy_workspace /opt/ros/groovy**

Para crear nuestro directorio utilizaremos el comando mkdir, de la forma:
**$ mkdir [espacio/de/trabajo]**

En nuestro ejemplo hemos decidido crear nuestro espacio de trabajo dentro de una carpeta llamada UPCT en el directorio groovy_workspace: 
**$ mkdir ~/groovy_workspace/UPCT**

Ahora procedemos a indicarle a nuestro sistema que este directorio recién creado va a ser un espacio de trabajo de ROS:
**$ rosws set ~/groovy_workspace/UPCT**

Ahora lo que hay que hacer es conﬁgurar el archivo .bash para indicarle a cada terminal donde debe trabajar:
**$ source ~/groovy_workspace/setup.bash**

Hay que destacar que deberemos de utilizar este último comando en cada uno de los terminales abiertos que queramos trabajar con nuestro sistema, o bien conﬁgurarlo dentro del repositorio general para que lo seleccione de forma automática. 

Para conﬁrmar que nuestro directorio lo reconoce ROS como un directorio válido de trabajo utilizaremos la función: 
**$ echo $ROS_PACKAGE_PATH**

A lo que veremos una pantalla parecida a esta:

#### c. Creando nuestro paquete
Ahora vamos a crear nuestro paquete, que será capaz de contener nuestro programa. Lo primero que vamos a hacer es acceder al espacio que hemos creado, para ellos usamos en nuestro caso la función: 
**$ cd ~/groovy_workspace/UPCT**

Ahora procedemos a crear el paquete que contendrá nuestro futuro programa: 
**$ roscreate-pkg UPCT_PFC std_msgs rospy roscpp 55**

Mediante esta función generamos un paquete llamado UPCT_PFC que depende de std_msgs, rospy y roscpp:

Ahora lo que vamos a hacer es comprobar que ROS es capaz de encontrar este nuevo paquete :  **$ rospack ﬁnd UPCT_PFC**

A lo que veremos en pantalla una respuesta como esta:  **/home/parallels/groovy_workspace/UPCT/UPCT_PFC**

Ahora procedemos a construir nuestro paquete y para ellos solo tenemos que introducir en nuestro terminal: **$ rosmake UPCT_PFC**

#### d. Preparando nuestro programa
Ahora vamos a hacer unos pasos opcionales pero altamente recomendables antes de empezar a crear nuestro programa, que es modiﬁcar los ﬁcheros Manifest.xml y Mainpage.dox En este caso Linux trae su propia función para editar estos documentos llamado gedit Primero accedemos a la carpeta contenedora :
**$ cd UPCT_PFC**

Ahora usamos la función descrita antes para modiﬁcar nuestro ﬁchero: 
**$ gedit manifest.xml
$ gedit mainpage.dox**

Estos ﬁcheros nos ayudan a tener una idea general del proyecto, de su autor y de su forma de funcionar, y puede ayudar a cualquier persona a saber si lo que busca lo va a encontrar en este paquete o no, así como mantener una forma de jerarquizar los paquetes iguales para todo el mundo.

#### e. Construyendo nuestro programa
Ahora que ya tenemos todo listo procedemos a crear nuestro ﬁchero ejecutable, para ello vamos a nuestro sistema de ﬁcheros la /UPCT_PFC / src, y le damos al botón derecho y pulsamos en crear un nuevo documento, documento en blanco. El siguiente paso es poner el nombre a nuestro ﬁchero en este caso lo llamaremos holamundo.cpp

A continuación abrimos el ﬁchero que acabamos de crear con un programa de edición de texto, o bien usando gedit tal y como lo hemos usado en el apartado anterior, y copiamos el siguiente código:

Tras introducir el código, lo guardamos y lo cerramos, y ahora procedemos a editar el ﬁchero CMakeList.txt y añadimos al ﬁnal de todo el código: 
**rosbuild_add_executable(hola_mundo src/holamundo.cpp)**

Esto hace que cuando generemos nuestro programa el sistema generará un ejecutable con el nombre hola_mundo, y cuyo código estará en la carpeta src/holamundo.cpp. 
Una vez realizado esto, debemos generar nuestro programa, para ello introducimos en nuestro terminal:  **$ make** 

Lo que nos tras unos segundos nos devolverá una salida por pantalla parecida a esta:

Así tendremos nuestro programa creado y listo para ser usado.

#### f. Arrancando nuestro programa
Una vez ya tenemos nuestro programa creado vamos a proceder a probarlo, para ello lo que hacemos es llamar a nuestro nodo tal y como hemos enseñado dentro del apartado correspondiente 
Lo primero que hay que hacer es llamar a nuestro nodo master, es decir, abrimos un nuevo terminal y ejecutamos 
**$ roscore**

Ahora volvemos a nuestro terminal primero en introducimos la función 
**$ rosrun UPCT_PFC hola_mundo**

Tras lo que veremos una salida por pantalla parecida a esta:

En el caso que no se inicie el programa, comprueba que tienes en una pantalla de terminal diferente activado roscore, y que en la pantalla con la que estás trabajando has ejecutado con anterioridad la función:

**$ source ~/groovy_workspace/setup.bash**

Ahora vamos a comprobar de forma gráﬁca que nuestro nodo está en funcionamiento, para ello abrimos una nueva pantalla de terminal y ejecutamos:  **$ rqt_graph**

### Conclusión
Como hemos podido ver a lo largo de todo el documento, el sistema ROS es un sistema robótico muy completo que nos permite utilizar tanto el código antiguo de otros proyectos, como uno nuevo generado directamente para nuestro sistema, además de contar con soporte para una gran multitud de robots y sensores existentes en el mercado, y otra de las ventajas de las que se ha hablado es de una gran comunidad que se está dedicando a mejorar día a día el sistema, así como de ampliar las compatibilidades tanto con sistemas nuevos (como puede ser Raspberry Pi), como con los últimos sensores y actuadores disponibles en el mercado. ROS es un sistema que en la actualidad cuenta con una gran cantidad de personas a nivel mundial que se dedican al mantenimiento y creación de nuevos repositorios, así como a la mejora del propio sistema, provocando una rápida adaptación a cualquier cambio.
Respecto a la compatibilidad, ROS es casi totalmente compatible con repositorios antiguos, lo que nos permite utilizar la programación que ya tenemos de otros sistemas y portarlos a este, permitiéndonos mover esta programación a casi cualquier máquina, y aquí  es donde podemos encontrar un el primer pero, ya que aunque la comunidad está trabajando fuertemente que se pueda utilizar en cualquier ordenador, a día de hoy solo pueden asegurar el correcto funcionamiento de ROS en sistemas GNU (Linux) y MAC OS X, y se están encontrando con algunos fallos de programación en sistemas Windows y Raspberry Pi, este último debido a que es un sistema totalmente nuevo y aún poco extendido. Cabe destacar que un sistema que está soportado por una gran comunidad tiene inﬁnidad de cosas positivas, pero también tiene varios apartados negativos, el primero de ellos es que al existir gran cantidad de repositorios, no todos tienen porque funcionar totalmente, y la solución a los errores de estos dependen también de la comunidad, lo que puede hacer que si es un repositorio que no sea usado normalmente, el fallo no sea descubierto de inmediato, y la corrección tarde en llegar; y otro de los principales problemas que puede suceder, es que hoy en día cualquier fundación o sistema de este tipo necesita unos recursos bastante abundantes que son muy difíciles de cubrir con donaciones, y con pequeñas contribuciones por parte de empresas privadas, lo que puede llevar a que en épocas de crisis o con una competencia fuerte las empresas y socios preﬁeran invertir ese dinero en otros sistemas, pudiendo llegar a la descontinuación de ROS provocando la migración obligatoria a otros sistemas.
Como futuros proyectos propuestos se podría dividir en dos vertientes, una más teórica, en la cual se pueden desarrollar robots en los entornos virtuales descritos en este documento, e incluso generar un Robot de los disponibles en los laboratorios, para comprobar que todo el programa funcionan de forma correcta,y una vertiente real, donde se vaya utilizando ROS para generar el código necesario para mover un robot real, al que se le pueden ir añadiendo más funciones con el paso del tiempo. Por supuesto estas dos vertientes pueden ser complementaria, ya que lo ideal sería generar un robot en el sistema virtual, probar que todo el código es completamente funcional, y luego cargarlo en nuestro robot real.

### Fuentes
○ www.ros.org   
○ www.willowgarage.com   
○ www.bipedolandia.es 
○ http://www.generationrobots.com/en/content/55-ros-robot-operating-system  
○ http://geeksroom.com/2013/08/ros-el-estandar-de-facto-de-la-industria-de-los-robots 
○ http://readwrite.com/2013/05/09/how-an-open-source-operating-system-jumpstartedrobotics-research#awesm=~ogKpiH3BrKRskJ  
○ http://robociencia.com/introduccion-a-ros/  
○ https://moodle2012-13.ua.es/moodle/mod/wiki/view.php?id=23601 
○ http://robociencia.com/ros-el-futuro-de-la-robotica-autonoma/ 
○ http://www.bipedolandia.es/t1654-explicacion-detallada-de-50-minutos-delfuncionamiento-de-kinect-y-ros-robot-operating-system  
○ http://www.automatizar.org/2011/09/creando-aplicaciones-para-robots.html  
○ http://www.instructables.com/id/Getting-Started-with-ROS-Robotic-Operating-Syste/  
○ ROS By Example GROOVY - Volume 1   Autor: R. Patrick Goebel  
○ http://es.wikipedia.org/wiki/Robótica 

