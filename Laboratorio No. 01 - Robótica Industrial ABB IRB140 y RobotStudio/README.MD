# Laboratorio 1: Robotica Industrial – Trayectorias, Entradas y Salidas Digitales
## Alejandro Ramirez - Ronan Anquetin - Nirvana Ceron
### Introduccion
El principal objetivo de este laboratorio era entender los principiode como funciona robots a nivel industrial, tanto a nivel de sus diversas formas de funcionamiento como en la operacion práctica, y finalmente como la combinacion de herramientas propias junto al uso del simulador de RobotStudio pueden unirse para que el robot pueda desarrollar tareas de gran complejidad con contrapartes potenciales a nivel industrial, o al menos contrapartes que requeririan este tipo de trabajo.
### Desarrollo

El primer paso para la realización de este laboratorio fue aprender a usar las herramientas para llevar la práctica a buen término, en este aspecto RobotStudio fue de lejos la más desafiante en virtud de que desde ahi es donde saldrán las tareas de mayor complejidad en lo que la práctica respecta.

El trabajo con la herramienta y el pastel fue más sencillo, al menos inicialmente. La herramienta fue creada en AutoCAD y despues impresa en 3D, pero a la hora de imprimir la rosca en la base de la herramienta no fue compatible con la parte de atras, tras varias consideraciones se optó por modificar la herramienta en si, usando pegamento y una botella para sacar un conjunto de rosca-agujero que estaba garantizado que fuera compatible, mas alla de eso la herramienta soporto las fuerzas que fueron aplicadas a ella, pero un problema parecido aparecio cuando se atornillo la herramienta al brazo robotico, por lo que solo se pudo atornillar con un agujero. 

La explicacion más probable para el problema es que fuera un defecto de la resolucion en la impresion de la herramienta, ya que estrictamente hablando todas las secciones de la herramienta estaban donde deberian y los tamaños eran correctos, el problema estaba en los grosores, lo que también hizo que fuera necesario remover el sticker del marcador para el que se habia diseñado originalmente.

En lo que respecta al robot se uso un robot ABB IRB 140, particularmente Cain, este tenia la banda transportadora mas baja que Abel, lo que dificulto marginalmente la simulacion hasta que se paso a un conjunto de configuraciones que fue capaz de llegar a todas las trayectorias sin sobrepasar los limites de cada articulacion.

### Resultados
Link del video en youtube: https://www.youtube.com/watch?v=ErBSSx0cb_A

El pastel fue decorado con éxito tras varias iteraciones del proceso en las que se corrigio por diferencias en la posicion e inclinacion del pastel en la banda transportadora respecto a la simulacion realizada en RobotStudio, posteriormente llego a su pose de mantenimiento y finalmente hizo su pose de aura, que en este caso fue moverse de lado a lado manteniendo la herramienta alineada.

Por las necesidades de tiempo se saltó directamente a la caracterizacion por modelo SAT para la herramienta, y se usó el mismo metodo para sacar los puntos para crear las trayectorias de la rutina para escribir en la mesa, la caracterizacion en si fue realizada con un modelo cad secundario, ya que el primario se corrompio y no se pudo sacar un archivo SAT a partir del STL (el STL son un monton de triangulos bidimensionales en vez de cuerpos sólidos, y por el chaflanano y roscado de las piezas no fue factible recrear la pieza más alla de las dimensiones necesarias para su caracterizacion.

El resultado de la herramienta recreada en SAT fue lo bastante bueno para que los unicos problemas salieran al compensar por el pastel y la banda transportadora, una vez el codigo dentro del .mod fue arreglado para cambiar las alturas y angulos de manera pertinente el grabado del pastel fue exitoso. 

### Referencias
Especificaciones de producto para robot ABB IRB 140. Disponible en: https://library.e.abb.com/public/a7121292272d40a9992a50745fdaa3b2/3HAC041346%20PS%20IRB%20140-en.pdf 


