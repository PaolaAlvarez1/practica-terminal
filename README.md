# practica-terminal

Ejercicio 0: Crear repositorio de github y activar servicio de codespaces.
Crear un repositorio de github llamado practica-terminal luego activar el servicio de Codespace según guia
https://scribehow.com/shared/Creacion_de_un_Nuevo_GitHub_Repositorio_y_Codespace__Vvlxr0dCTgqhoohNe7VtqA
y https://scribehow.com/shared/como_detener_un_GitHub_Codespace__ppnNOPHyTWCFxKpniGLow suministrada
por el instructor.
Después de ello desarrollar los Ejercicios evacuativos planteado a continuación, creando la respectiva evidencia.
Ejercicio 1: Navegación y Visualización de Directorios
Objetivo:
Utilizar los comandos ls , cd y pwd para explorar y visualizar la estructura de directorios.
Instrucciones:
 Abre una terminal y, partiendo de tu directorio personal, realiza lo siguiente:
Ejecuta pwd para mostrar tu ruta actual.
Utiliza ls -l para listar el contenido del directorio.
Cambia a un directorio existente (por ejemplo, cd Documentos o el que tengas en tu sistema) y vuelve a ejecutar
pwd para confirmar la nueva ubicación.
Regresa a tu directorio inicial con cd ~ .
Evidencia a Entregar:
Capturas de pantalla o un registro de la terminal que muestre:
La salida del comando pwd antes y después del cambio de directorio.
La salida del comando ls -l en ambos directorios.
Ejercicio 2: Creación y Manipulación de Archivos y Directorios
Objetivo:
Crear y organizar una estructura de directorios y archivos, y luego manipularlos utilizando mkdir , touch , cp , mv y rm .
Instrucciones:
 En tu directorio de trabajo, crea una carpeta llamada ProyectoCLI :
 Dentro de ProyectoCLI , crea dos subdirectorios: src y docs .
 En el directorio docs , crea un archivo llamado README.txt utilizando solo la terminal.
 Agrega contenido al archivo README.txt (puedes usar un editor de texto o redirigir una línea de texto, por ejemplo:
echo "Este es el README del ProyectoCLI"
 Copia el archivo README.txt al directorio src :
 Renombra el archivo copiado en src a INFO.txt .
 Finalmente, elimina el directorio docs completo.
Evidencia a Entregar:
Una captura de pantalla o registro de terminal que muestre:
Prueba técnica de manejo de Terminal. 1
La creación de la estructura de directorios.
La ejecución de los comandos de copia, renombrado y eliminación.
La estructura final de directorios luego de eliminar docs .
Ejercicio 3: Enlaces Simbólicos y Manejo de Rutas
Objetivo:
Crear y gestionar enlaces simbólicos y extraer información de rutas utilizando ln -s , readlink , basename y dirname .
Instrucciones:
 En tu directorio de trabajo, crea un archivo de prueba llamado archivo_original.txt con algo de contenido:
 Crea un enlace simbólico llamado enlace.txt que apunte a archivo_original.txt :
 Utiliza readlink para verificar a qué archivo apunta el enlace.
 Emplea basename y dirname sobre la ruta completa de archivo_original.txt para extraer el nombre del archivo y el
directorio que lo contiene.
Evidencia a Entregar:
Capturas de pantalla o registro de la terminal que muestren:
La creación del archivo y del enlace simbólico.
La salida de readlink enlace.txt .
Los resultados de basename y dirname .
Ejercicio 4: Búsqueda y Filtrado de Archivos
Objetivo:
Utilizar comandos de búsqueda como find , locate (junto con updatedb ) y whereis para encontrar archivos y ubicaciones
de ejecutables.
Instrucciones:
 Utiliza find para buscar todos los archivos con extensión .txt dentro de tu directorio actual:
 Actualiza la base de datos de locate con sudo updatedb (si es necesario) y luego utiliza locate para buscar el mismo
archivo de prueba archivo_original.txt .
 Usa whereis para encontrar la ubicación de un comando común (por ejemplo, bash ):
Evidencia a Entregar:
Capturas de pantalla o registro de la terminal que muestren:
La salida del comando find .
La salida de locate para archivo_original.txt .
La salida de whereis bash .
Ejercicio 5: Visualización y Redirección de Contenido
Objetivo:
Utilizar los comandos cat , less , more y tee para visualizar y redirigir el contenido de archivos.
Instrucciones:
 Visualiza el contenido de archivo_original.txt .
Prueba técnica de manejo de Terminal. 2
 Abre el mismo archivo y desplázate por el contenido.
 Utiliza more para visualizar el archivo nuevamente.
 Redirige la salida del comando cat archivo_original.txt hacia un nuevo archivo llamado copia.txt usando tee :
Evidencia a Entregar:
Capturas de pantalla o registros de terminal que incluyan:
La salida de cat , less y more .
La creación y contenido de copia.txt tras usar tee .
Ejercicio 6: Gestión de Atributos y Eliminación Segura
Objetivo:
Modificar atributos de archivos con chattr y lsattr , y eliminar un archivo de forma segura con shred .
Instrucciones:
 Selecciona un archivo de prueba (por ejemplo, copia.txt ) y aplica el atributo inmutable utilizando chattr :
 Verifica los atributos del archivo con lsattr copia.txt .
 Intenta modificar o eliminar el archivo para constatar que el atributo está activo.
 Luego, remueve el atributo inmutable:
 Finalmente, utiliza shred para eliminar copia.txt de forma segura:
Evidencia a Entregar:
Capturas de pantalla o registro de la terminal que muestren:
La aplicación y verificación de los atributos con chattr y lsattr .
El intento fallido de modificar/eliminar el archivo con el atributo inmutable.
La ejecución de shred y la confirmación de eliminación.
Ejercicio 7: Script Interactivo con read
Objetivo:
Crear un script sencillo que capture entrada del usuario y la utilice para generar una respuesta.
Instrucciones:
 Crea un archivo de script llamado saludo.sh y añade el siguiente contenido (o similar):
#!/bin/bash
echo "Por favor, ingresa tu nombre:"
read nombre
echo "Hola, $nombre. ¡Bienvenido al mundo de la línea de comandos!"
 Dale permisos de ejecución al script:
 Ejecuta el script y responde a la solicitud de entrada.
Evidencia a Entregar:
El contenido del script saludo.sh (puede ser mediante una captura de pantalla del editor o el comando cat saludo.sh ).
La ejecución del script mostrando la interacción y la respuesta del programa.
