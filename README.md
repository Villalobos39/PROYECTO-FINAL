# PROYECTO-FINAL: Sistema Operativo Robótico

## ROS (Robot operating system).

Para poder sacar el máximo rendimiento a ROS, primero tenemos que comprender en qué consiste el sistema, y cuales son sus principales ventajas respecto al resto de sistemas que se pueden encontrar hoy en día. Un robot es una máquina controlada por ordenador y programada para moverse, manipular objetos y realizar trabajos a la vez que interacciona con su entorno.

#### Los robots exhiben tres elementos claves según la deﬁnición adoptada

Capacidad mecánica, que lo capacita para realizar acciones en su entorno y no ! ser un mero procesador de datos . Flexibilidad, puesto que el robot puede operar según un amplio rango de ! programas y manipular material de formas distintas. La idea más ampliamente aceptada de robot está asociada a la existencia de un dispositivo de control digital que, mediante la ejecución de un programa almacenado en memoria, va dirigiendo los movimientos de un brazo o sistema mecánico.

### ¿ Qué es ROS ?

Es similar a otras plataformas de desarrollo para robots existentes en la actualidad, y su mayor virtud, es la de haber sabido aunar lo mejor de cada uno de estos sistema, juntando todo en un solo sistema capaz de comunicarse tanto con los robots mas modernos, como con los ya existentes en el mercado. Desde su creación, ROS se ha diseñado para facilitar el intercambio de software entre los aﬁcionados y los profesionales de la robótica en todo el mundo debido a su enfoque didáctico y abierto, lo que ha permitido la construcción de una gran comunidad de colaboradores a lo largo de todo el mundo. 

### El objetivo de ROS
El objetivo de ROS no es ser un sistema pionero en la robótica, el objetivo principal de ROS es apoyar el código reutilizable en la investigación robótica y el desarrollo. El sistema es una estructura distribuida en procesos que permite a los ejecutables ser diseñados de forma individual y utilizarse de forma ﬂexible en tiempo real.

El objetivo principal de este proyecto es el de compartir y colaborar, pero hay varios objetivos más dentro del marco ROS:
Sencillez: ROS está diseñado para ser tan sencillo como sea posible de modo que el código escrito para ROS se pueda utilizar con otros marcos robot de software. ROS es fácil de integrar con otros sistemas operativos de robots y ya ha sido integrado con OpenRAVE, Orocos y Player. 

Modelo de bibliotecas: es el modelo de desarrollo preferido, consiste en escribir una serie de programas con interfaces funcionales y limpias que permitan una rápida modiﬁcación. 

### Compatibilidad con los sistemas operativos 
ROS también es compatible con el sistema de repositorios, que permiten la colaboración a nivel internacional permitiendo tomar decisiones independientes sobre el desarrollo y la ejecución, pero con la ventaja de poder ayudarse de las herramientas o archivos creados por otros en sus proyectos.

ROS es fácil de integrar con otros sistemas operativos de robots y ya ha sido integrado con OpenRAVE, Orocos y Player. Sistemas operativos admitidos. ROS en la actualidad sólo se ejecuta de forma totalmente funcional en plataformas basadas en UNIX. el Software de ROS está principalmente probado en Ubuntu y Mac OS X, aunque la comunidad ROS ha contribuido al apoyo a Fedora, Gentoo, Arch Linux y además de otras plataformas Linux.

Respecto a Microsoft Windows, es un sistema en el que podremos instalar nuestro sistema ROS, aunque todavía existen algunos pequeños errores que se están intentando solucionar. Nuevas bibliotecas. Tanto el núcleo del sistema ROS, como los útiles, herramientas y bibliotecas son creados y actualizados regularmente como una distribución de ROS . Esta distribución es similar a una distribución de Linux y ofrece un conjunto de software compatible para que todo el mundo pueda usarla, además de que por su naturaleza Open Source te permite modiﬁcar cualquier distribución para poder adaptarla a tus necesidades.

### Funcionamiento del sistema
ROS tiene tres niveles de conceptos: el nivel del sistema de archivos, el nivel de Computación Gráﬁca, y el nivel comunitario. Estos niveles y conceptos se resumen a continuación.

### Sistema de archivos.
Son recursos que se encuentran en el propio programa: 
○ Paquetes: Los paquetes son la unidad principal para organizar software en ROS. Un paquete puede contener procesos ejecutables (nodos), una biblioteca dependiente, conjuntos de datos, archivos de conﬁguración, o cualquier otra cosa que sea útil para una organización conjunta. 
○ Maniﬁestos: proporcionan metadatos sobre un paquete, incluyendo su información de licencia y dependencias, así como información especíﬁca del compilador. 
○ Pilas: Es una colección de paquetes que tienen una misma función. 
○ Maniﬁestos de pilas: proporcionan datos sobre una pila, incluyendo su información de licencia y sus dependencias en otras pilas.
○ Mensajes: deﬁnen las estructuras de datos para los mensajes enviados en ROS.
○ Servicios:  deﬁnen la solicitud y estructuras de datos de respuesta de los servicios requeridos por ROS.

### Computación a nivel Gráﬁco. 
La computación a nivel gráﬁco es la red ROS que se encarga de procesar todos los datos. Un sistema de control de robot comprenderá usualmente muchos nodos.

Por ejemplo, un nodo controla un telémetro láser, un nodo controla los motores de las ruedas, un nodo realiza localización, un nodo realiza la planiﬁcación de ruta, un nodo proporciona una vista gráﬁca del sistema, y así sucesivamente. Sin el Maestro, los nodos no serían capaces de encontrar mensajes entre sí, intercambiar, o invocar los servicios. Un mensaje es simplemente una estructura de datos que comprende los tipos de campos. Los mensajes pueden incluir estructuras arbitrariamente anidadas y matrices .

Un nodo envía un mensaje por publicar a un determinado tema. Un nodo que está interesado en un determinado tipo de datos se suscribe al tema correspondiente. Puede haber varios editores y suscriptores concurrentes a un mismo tema, y un único nodo puede publicar y / o suscribirse a múltiples temas. La comunidad y ROS.

Los conceptos comunitarios ROS Nivel ROS son recursos que permiten a las comunidades el intercambio del software y del conocimiento.
