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
´´´ bash 
![image](https://github.com/user-attachments/assets/eb1d4bbe-220f-4575-aeb8-27be9d97592e)
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mkdir -p ProyectoCLI/{Src,Docs}
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ touch ProyectoCLI/Docs/readme.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ echo "Este es el proyecto README del ProyectoCLI" > ProyectoCLI/Docs/readme.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ cp ProyectoCLI/Docs/readme.txt ProyectoCLI/Src
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ mv ProyectoCLI/Src/readme.txt  ProyectoCLI/Src/Info.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ rm -r ProyectoCLI/Docs
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ 
´´´
## EJERCICIO #3: Enlaces Simbólicos y Manejo de Rutas
´´´ bash 
![image](https://github.com/user-attachments/assets/d167b59c-3056-4b89-9514-86fc95bccbc5)
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ readlink -f enlace.txt
/workspaces/practica-terminal/archivo_orginal.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ basename "$(realpath archivo_original.txt)"
archivo_original.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls-l
bash: ls-l: command not found
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls -l
total 40
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:40 -
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 Documentos
drwxrwxrwx+ 5 codespace codespace 4096 Feb 20 23:47 MyDirectory
drwxrwxrwx+ 3 codespace codespace 4096 Feb 21 00:12 ProyectoCLI
-rw-rw-rw-  1 codespace root      6071 Feb 20 23:25 README.md
-rw-rw-rw-  1 codespace codespace   18 Feb 21 00:25 archivo_original.txt
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 cd
lrwxrwxrwx  1 codespace codespace   19 Feb 21 00:26 enlace.txt -> archivo_orginal.txt
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:40 p
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:26 prueba
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ 
´´´
## EJERCICIO #4: Ejercicio 4: Búsqueda y Filtrado de Archivos
´´´ bash
![image](https://github.com/user-attachments/assets/fdc7cc07-daa9-43b1-8814-4f5496b80731)
![image](https://github.com/user-attachments/assets/0226bc4d-328c-4447-ad23-114670298f21)

@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ readlink -f enlace.txt
/workspaces/practica-terminal/archivo_orginal.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ basename "$(realpath archivo_original.txt)"
archivo_original.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls-l
bash: ls-l: command not found
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ ls -l
total 40
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:40 -
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 Documentos
drwxrwxrwx+ 5 codespace codespace 4096 Feb 20 23:47 MyDirectory
drwxrwxrwx+ 3 codespace codespace 4096 Feb 21 00:12 ProyectoCLI
-rw-rw-rw-  1 codespace root      6071 Feb 20 23:25 README.md
-rw-rw-rw-  1 codespace codespace   18 Feb 21 00:25 archivo_original.txt
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:27 cd
lrwxrwxrwx  1 codespace codespace   19 Feb 21 00:26 enlace.txt -> archivo_orginal.txt
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:40 p
drwxrwxrwx+ 2 codespace codespace 4096 Feb 20 23:26 prueba
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ find . -type f -name "*.txt"
./ProyectoCLI/Src/Info.txt
./archivo_original.txt
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ sudo updatedb
sudo: updatedb: command not found
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ locate archivo_original.txt
bash: locate: command not found
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ find
.
./cd
./-
./enlace.txt
./Documentos
./.git
./.git/hooks
./.git/hooks/post-update.sample
./.git/hooks/applypatch-msg.sample
./.git/hooks/fsmonitor-watchman.sample
./.git/hooks/update.sample
./.git/hooks/pre-applypatch.sample
./.git/hooks/commit-msg.sample
./.git/hooks/pre-merge-commit.sample
./.git/hooks/pre-commit.sample
./.git/hooks/pre-rebase.sample
./.git/hooks/pre-push.sample
./.git/hooks/pre-receive.sample
./.git/hooks/push-to-checkout.sample
./.git/hooks/sendemail-validate.sample
./.git/hooks/prepare-commit-msg.sample
./.git/description
./.git/lfs
./.git/lfs/tmp
./.git/FETCH_HEAD
./.git/HEAD
./.git/objects
./.git/objects/c0
./.git/objects/c0/938e52d535e649f2633344fb5e64a65adc27f5
./.git/objects/pack
./.git/objects/pack/pack-a6401511c9d048e3a18b34e2b5d06f1ec07561c1.pack
./.git/objects/pack/pack-a6401511c9d048e3a18b34e2b5d06f1ec07561c1.rev
./.git/objects/pack/pack-a6401511c9d048e3a18b34e2b5d06f1ec07561c1.idx
./.git/objects/03
./.git/objects/03/21bb78ec693f8b9c798153556f7ca6d4bf32f0
./.git/objects/info
./.git/objects/8c
./.git/objects/8c/21548258877eba4d673dfa45449ac81218f510
./.git/info
./.git/info/exclude
./.git/refs
./.git/refs/heads
./.git/refs/heads/main
./.git/refs/tags
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/refs/remotes/origin/HEAD
./.git/logs
./.git/logs/HEAD
./.git/logs/refs
./.git/logs/refs/heads
./.git/logs/refs/heads/main
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/logs/refs/remotes/origin/HEAD
./.git/index
./.git/config
./.git/packed-refs
./.git/branches
./prueba
./ProyectoCLI
./ProyectoCLI/Src
./ProyectoCLI/Src/Info.txt
./archivo_original.txt
./p
./README.md
./MyDirectory
./MyDirectory/Codigo
./MyDirectory/ProyectoCLI
./MyDirectory/Recursos
./MyDirectory/Backup
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ whereis bash
bash: /usr/bin/bash /etc/bash.bashrc /usr/share/man/man1/bash.1.gz
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ whereis python
python: /usr/bin/python3.8-config /usr/bin/python3.8 /usr/lib/python3.8 /usr/lib/python2.7 /usr/lib/python3.9 /etc/python3.8 /usr/local/lib/python3.8 /usr/include/python3.8 /usr/local/python /opt/conda/bin/python /opt/conda/bin/python3.12 /opt/conda/bin/python3.1 /opt/conda/bin/python3.12-config /usr/local/python/3.12.1/bin/python /usr/local/python/3.12.1/bin/python3.12 /usr/local/python/3.12.1/bin/python3.12-config
@PaolaAlvarez1 ➜ /workspaces/practica-terminal (main) $ 
´´´
