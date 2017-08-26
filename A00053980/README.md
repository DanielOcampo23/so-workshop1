# Taller 1

**Nombre:** Daniel Steven Ocampo  
**Código:** A00053980  

## Descripción 
Mediante este taller estudiaremos algunos directorios y archivos mas importantes que se encuentran en la carpeta raíz de linux, también se mencionarán algunos comandos no vistos en la clase de sistemas operativos, y por ultimo aprenderemos a utiliazar viables de ambiente en un Sistema Linux.
## Soluciones

### 1.  

| Directorio   | Archivo ejemplo | Descripción del contenido del directorio  |
|------|------|------|
| usr   |   games   | En la carpeta "usr" se encuentran la mayoria de los archivos de un sistema Linux, como ejecutables, documentación, etc... Un ejemplo de esto, es la carpeta "games" en donde claramente se encuentran todos los ejecutables de los juegos del sistema como por ejemplo ```espdiff```, ```gnome-mahjongg```, ```gnome-mines```, ```gnome-sudoku```,   ```sl```, ```sl-h```, ```sol``` .|
| bin   |   sleep , cat  | En la carpeta "bin" se encuentran los Ejecutables (o binarios) básicos del sistema, cuando, por ejemplo ejecutamos el comando cp en realidad ejecutamos /bin/cp. El archivo ejemplo dentro de esta carpeta es ```sleep``` como lo indica su nombre "duerme" el sistema durante los segundos que le indique el usuario. También se encuentra el archivo ```cat``` que es usado muy usualmente por los usuarios que utilizan linux y sirve para mostrar el contenido de un archivo en la misma terminal si necesidad de utilizar ningun editor de texto. | 
| home   | daniel  | En la carpeta "home" se encuentran todas las carpetas de cada usuario del sistema por ejemplo en mi caso en particular se encuentra la carpeta "daniel" en la cual se encuentran todas mis carpetas como "Documentos", "Descargas", etc..  |
| tmp   |  --- | En la carpeta "tmp" como su abreviación lo menciona es una carpeta temporal, por esta razón los archivos que se agregan en esta carpeta se eliminan cuando se apaga y se vuelve a prender el sistema  |
| etc   |  group, protocols  | En la carpeta "etc" se encuentran los archivos básicos de configuracin, en donde podemos encontrar el archivo ```group``` el cual es una lista de grupos del sistema, y también podemos encontrar ```protocols``` el cual también es una lista de protocolos de internet que soporta la maquina.     |
| root   |  --- | Esta es la carpeta privada del root, aquí puede guardar los archivos personales.  |
| boot   |  abi-4.4.0-31-generic |  Archivos estáticos utilizados por el cargador de arranque(boot-loader) del sistema.  |
| lib   | init/stab |  Estos ficheros contienen código que compartirán muchos programas. En lugar de que cada programa contenga una copia propia de las rutinas compartidas, éstas son guardadas en este fichero. Esto hace que los programas ejecutables sean menores y reduce el espacio usado en disco. |
| var   |  spool/mail   | Este directorio contiene información temporal de los programas (lo cual no implica que se pueda borrar su contenido) , por ejemplo spool/mail como veiamos en clase allí llegan los correos de las personas que trataron a acceder a un usuario no permitido |
| media   | ----  |  Puntos de montaje para dispositivos de medios, como son las unidades lectoras de discos compactos  |
| dev   | cpu_dma_latency  | Contiene archivos especiales del sistema, conocidos como controladores de dispositivo (device drivers), los cuales se usan para acceder a los dispositivos del sistema y recursos, como discos duros, modems, memoria, etc.  |
| opt   | google/chrome | Aplicaciones adicionales  |
| mnt   |  --- | Sistemas de archivos montados manualmente en el disco duro  |
| proc   |  bus | Información del sistema usada por el kernel. Por ejemplo ```bus``` Información sobre los buses instalados|
| run   |  docker | Está diseñado para permitir que las aplicaciones puedan almacenar los datos que se requieran para operar  |
| srv   | --- | Puede contener archivos que se sirven a otros sistemas  |
| sys   |  kernel |  Al igual que /proc, contiene archivos virtuales que proveen información del kernel relativa a eventos del sistema operativo. Es en cierto modo una evolución de /proc, y a diferencia de este último, los archivos se distribuyen de forma jerárquica. |

### 2.  

2. En una tabla como se muestra a continuación escriba 10 comandos de Linux no visto en clase. Puede incluir comandos que funcionan una vez han sido instalados con yum

| Comando   | Usuario | Descripción   |
|------|------|------|
| cp | root | Copia un archivo de un directorio a otro  |
| logout | root | cierra la sesión   |
| reboot | root | Reinicia el sistema  |
| tree | root | Muestra los directorios y los ficheros en forma de arbol comenzando por la raíz (carpeta en donde esta parado el usuario)  |
| rar a fichero.rar | root | crea un fichero "rar" llamado "fichero.rar" |
| find [patron] | root | Busca las coincidencias con el patron dentro del directorio y sus subdirectorios  |
| rm -r | root | Eliminar un directorio recursivamente  |
| date | root |  Muestra la hora y la fecha en formato completo  |
| clear | root | limpia todos los comandos escritos en la teminal  |
| reset | root | reinicia la terminal  |



### 3.  

El comando ```printenv``` sirve para mostrar la lista de variables de ambiente del sistema, con el comando "export" podemos agregar variables de ambiente a esta lista que aparece con el comando ```printenv``` un ejemplo de esto es ```export VARIABLE=DANIEL```

Para que las variables de ambiente sean permanentes en el sistema se ejecuta de la siguiente manera ```sed '$ a export VARIABLE=DANIEL' /etc/profile``` siguiente a esto se reinicia el sistema para revisar si la variable queda permanente 


### 4.  
### 5.  

## Referencias
http://www.mancera.org/2011/06/26/%C2%BFque-contiene-cada-carpeta-de-linux/

http://www.rinconsolidario.org/linux/cursoLinux/comoUsarLinux/directorios/directorios.html

https://computernewage.com/2015/06/14/el-arbol-de-directorios-de-linux-al-detalle-que-contiene-cada-carpeta/

https://github.com/ICESI/all-workshops/blob/master/2017_b/so/workshop1/README.md

https://github.com/ICESI/so-commands/tree/master/centos7
