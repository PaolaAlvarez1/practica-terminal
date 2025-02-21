## EJERCICIO #1 NAVEGACION Y VISUALIZACION DE DIRECTORIOS
´´´ bash
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ pwd
/workspaces/practica-terminal
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mkdir prueba
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls -l
total 12
-rw-rw-rw-  1 codespace root      6071 Feb 20 23:25 README.md
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:26 prueba
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mkdir cd Documentos
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls -l
total 20
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 Documentos
-rw-rw-rw-  1 codespace root      6071 Feb 20 23:25 README.md
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 cd
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:26 prueba
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ pwd
/workspaces/practica-terminal
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ cd ~
@PaolaAlvarez1 ➜ ~ $ 
´´´
## EJERCICIO #2 : Creación y Manipulación de Archivos y Directorios
´´´ bash ![image](https://github.com/user-attachments/assets/eb1d4bbe-220f-4575-aeb8-27be9d97592e)
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mkdir -p ProyectoCLI/{Src,Docs}
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ touch ProyectoCLI/Docs/readme.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ echo "Este es el proyecto README del ProyectoCLI" > ProyectoCLI/Docs/readme.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ cp ProyectoCLI/Docs/readme.txt ProyectoCLI/Src
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mv ProyectoCLI/Src/readme.txt  ProyectoCLI/Src/Info.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ rm -r ProyectoCLI/Docs
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ 
´´´

