<p align="center">

&#x20; <img src="https://img.shields.io/badge/Linux-Terminal-black?style=for-the-badge\&logo=linux">

&#x20; <img src="https://img.shields.io/badge/Bash-Scripting-green?style=for-the-badge\&logo=gnubash">

&#x20; <img src="https://img.shields.io/badge/GitHub-Portfolio-blue?style=for-the-badge\&logo=github">

</p>




### explicación el paso a paso de creación de un archivo por medio de una terminal de Ubuntu, donde se cree un directorio, luego, un archivo donde se escriba algo, se modifique, luego se mueva de carpeta y se elimine

En la gestion de archivo en una terminal de windows los comando son similares, a los de el terminal de Linux. En este caso se visualizara la creación, edición, mover el archivo de carpeta y luego se elimine. 

Por lo tanto se visualizara aquellos comando para realizarlos en la terminal Linux 

Lista de comandos:
- mkdir
- cd 
- cd .. 
- mv 
- rm -r
- rmdir 

#### mkdir

Comando utilizado para crear carpetas o subcarpetas.

#### cd
Comando utilizado para conocer la ruta en la cual se encuentra ubicado **cd**, si quiere acceder a una carpeta de utiliza el comando **cd Nombre_carpeta** . si quiere devolverse al anterior carpeta se utiliza **cd ..** 

#### mv

Se utiliza para mover el archivo de una carpeta a otra, hay que tener en cuenta que la ubición donde se encuentra posiciona archivo a mover, por lo tanto se dirige a la capeta y utilia el comando **mv nombre_carpeta_inicial** despues **nombre_carpeta_final**, este mismo comando se utiliza para poder renombrar un archivo por lo tanto, se considera con la misma estructura, ejemplo **mv nombre_archivo_inicial** despues **nombre_archivo_final**

#### rm -r

Se utiliza para eliminar carpetas que no importa si estan vacias o no, si se quiere eliminar un solo archivo es rmdir **nombre_archivo**


#### Ejemplo practico : 


Es importante reconocer hay dentro de cada carpeta, que archivos o elementos hay, en el lugar que este ubicado, para ello, se utiliza el comando **ls -l**, como se evidencia en la siguiente imagen.

![Paso 2](https://github.com/Sergio-116/PROYECTO_LINUX/blob/f34cd6e64894879cd176013e319eaaf4a492f979/IMAGENES/02_ArchivoLogs.png)

En la gestión de archivos también se puede necesitar encontrar un archivo dentro de una carpeta, tenga en cuenta que solo buscara en dicha carpeta donde este ubicado, sea el caso de tener una carpeta dentro en la que usted se encuentra, no va a buscar, el comando para realizar esta búsqueda es **find _El nombre del archivo junto con la extención_**. 

Es menester hablar de como retroceder a la carpeta anterior, crear nuevo archivo vacio, es decir sin nada de contenido, en los comando utilizados son **cd ..* y **touch nombre del archivo*

![Paso 3](https://github.com/Sergio-116/PROYECTO_LINUX/blob/f34cd6e64894879cd176013e319eaaf4a492f979/IMAGENES/03_UsoNano.png)

Guardar un respaldo es tan importante como desarrollar en cualquier ámbito, por tal razón, **cp combre del archivo ../Carpeta a donde quiere hacer backup/**, en este caso se realizo una carpeta adentro de la carpeta Practica_Linux en la misma gerarquia de la carpeta Documentos, de este modo se realizo el Backup. 

![Paso 4](https://github.com/Sergio-116/PROYECTO_LINUX/blob/f34cd6e64894879cd176013e319eaaf4a492f979/IMAGENES/04_RealizacionBackup.png)


En su momento todo debemos realizar un cambio de nombre a algún archivo, el comando utilizado en Linux **mv nombre_inicial nombre_final** se evidencia en la siguiente imagen

![Paso 5](https://github.com/Sergio-116/PROYECTO_LINUX/blob/f34cd6e64894879cd176013e319eaaf4a492f979/IMAGENES/05_Cambiar_nombre.png)

Para eliminar un documento o carpeta hay dos maneras de llevar a cabo **rmdir nombre** y **rm -r nombre ** de la segunda manera se elimina aquello que se halla seleccionado

![Paso 6](https://github.com/Sergio-116/PROYECTO_LINUX/blob/f34cd6e64894879cd176013e319eaaf4a492f979/IMAGENES/06_ConfiguacionPermisos.png)



### ¿Cuáles son los pasos para crear repositorio remoto, sincrinizar, clonar a nivel local, para luego subir infromación y corroborar se estado a través de la terminal de github bash?


1. Paso inicial, se crea el repositorio desde la web ingresando al git hub 
2. después se debe copiar la URL del repositorio 
3. En la carpeta deseada se debe iniciar el **git init**
4. git clone https://URL_repositorio.git
5. Se lista que clono y prosede a crear las carpetas que de desee
6. se crea el archivo **type nul > archivo.md**
7. git add .
8. git commit -m "Primer commit"
9. git remote add origin URL
10. git push -u origin main


###¿Cuál es la diferencia entre las diferentes topologías de RAID?, explique con un esquema cada arquitectura y su funcionamiento. 

Imagen mapa conceptual dibujo 

 

####¿Qué es Docker? y ¿qué es una máquina virtual?, comentar las características y arquitectura de cada una, además de sus diferencias y aplicaciones. 

####¿Qué es una Máquina Virtual (VM)? 

Una Máquina Virtual es una emulación de un ordenador físico. Funciona sobre un software llamado Hipervisor, que reparte los recursos de hardware (CPU, RAM, Disco) para crear instancias aisladas. 

##### Características: 

Hardware: El servidor físico real. 

Hipervisor: La capa de software (como VMware o VirtualBox) que gestiona las VMs. 

Sistema Operativo Invitado (Guest OS): Cada VM incluye una copia completa de un sistema operativo (Windows, Linux, etc.), con sus propios drivers y binarios. 

Aislamiento total: Si una VM falla o es atacada, las demás no se ven afectadas. 

Pesadas: Consumen muchos recursos porque cada una debe arrancar un SO completo. 

 

### ¿Qué es Docker (Contenedores)? 

Docker es una plataforma que permite empaquetar una aplicación y todas sus dependencias en un contenedor. A diferencia de las VMs, los contenedores comparten el núcleo (kernel) del sistema operativo anfitrión. 

Características: 

Infraestructura: El servidor físico o virtual. 

Sistema Operativo Host: Normalmente una distribución de Linux. 

Docker Engine: La capa que gestiona los contenedores. 

Binarios y Librerías: Solo lo necesario para que la aplicación funcione. No hay un SO invitado. 

Ligeros: Pesan megabytes en lugar de gigabytes. 

 

Diferencias Clave 

 

Características 

Máquina Virtual (VM) 

Docker (Contenedores) 

Aislamiento 

Aislamiento a nivel de Hardware. 

Aislamiento a nivel de Proceso/SO. 

Peso 

GBs (Incluye todo el SO). 

MBs (Solo app y librerías). 

Rendimiento 

Menor (emulación de hardware). 

Casi nativo. 

Escalabilidad 

Difícil y lenta. 

Muy fácil y rápida. 

SO compatible 

Puedes correr Windows sobre Linux. 

Deben compartir el kernel del host. 

 

 

 

### Aplicaciones y Casos de Uso 

¿Cuándo usar Máquinas Virtuales? 

Las Máquinas Virtuales son la opción ideal cuando se requiere ejecutar aplicaciones en un sistema operativo distinto al del servidor (como una app de Windows sobre Linux), ya que proporcionan un entorno totalmente independiente. Asimismo, su arquitectura garantiza un aislamiento de seguridad extremo y ofrece la robustez necesaria para gestionar infraestructuras de nube complejas de manera eficiente. 

¿Cuándo usar Docker? 

Docker es la solución perfecta para implementar microservicios, permitiendo dividir aplicaciones en piezas independientes que facilitan el escalado dinámico de cientos de instancias en segundos. Además, optimiza los entornos de desarrollo al asegurar que todos los programadores utilicen la misma configuración y agiliza los procesos de CI/CD mediante la automatización eficiente de pruebas y despliegues.  

 

### ¿Cuáles son las capas del modelo OSI?, explicar cada una y dar ejemplos reales de aplicación. 

 

El Modelo de Interconexión de Sistemas Abiertos (OSI) es un marco conceptual creado por la ISO que estandariza las funciones de un sistema de telecomunicaciones en siete capas distintas. Se lee generalmente de abajo hacia arriba (desde el hardware hasta el usuario). 

 

Capa Física (Physical Layer) 

 

Es la capa de hardware. Se encarga de la transmisión y recepción de bits puros a través de un medio físico (cables, ondas de radio, fibra óptica). 

 

Función: Define voltajes, velocidades de datos y conectores físicos. 

Ejemplo real: Cables Ethernet (RJ45), repetidores, hubs y el estándar Bluetooth. 

 

Capa de Enlace de Datos (Data Link Layer) 

 

Proporciona el direccionamiento físico y la detección de errores en la transmisión bloque a bloque (tramas). 

 

Función: Gestiona el acceso al medio y el direccionamiento MAC. 

Ejemplo real: El protocolo Ethernet (a nivel de switch), el protocolo Wi-Fi (802.11) y las direcciones MAC de tus dispositivos. 

 

Capa de Red (Network Layer) 

 

Se encarga de determinar la mejor ruta para que los datos lleguen de un punto A a un punto B (enrutamiento). 

 

Función: Gestiona el direccionamiento lógico y la fragmentación de paquetes. 



##### Parcial realizado por Johan Andres Paez Garzón, David Santiago Prada Briceño y Sergio Quintana

