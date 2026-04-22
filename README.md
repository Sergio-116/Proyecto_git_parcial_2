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

