# Comandos Básicos de Git.
## Iniciar Repositorio
Iniciar un nuevo repositorio, agregar los archivos y generar una entrada en la BD local de git. Luego de este paso lo que se hace es ir agregando entradas con ``` git add ``` especificando el nombre del archivo a agregar o `.` para que agregue todo el contenido de la carpeta y seguir haciendo commits.

    1. git init
    2. git add Comandos Git.md | git add .
    3. git commit -m 'Mensage o descripcion'

## Obteniendo informacion sobre los archivos rastreados.
### Comando:
    1. git status
    2. git log  Comandos Git.md
    3. git show Comandos Git.md
    4. git diff f037bd8d1e3a9ec662ff19dd28b79e6ec616d74c 3a12197528d37295480c77038b84aeabc29106e4

### Descripción:
    1. Muestra el estado actual del repositorio.
    2. Muestra el registro de todos los commits aplicados sobre el archivo.
    3. Hace una comparacion entre las versiones de los archivos y muestra los cambios.
    4. Compara dos commits y muestra los cambios, el orden de los commits es importante

## Moviendonos entre versiones
### Comandos:
    1. git reset f037bd8d1e3a9ec662ff19dd28b79e6ec616d74c [ --soft | --hard ]
    2. git checkout [ f037bd8d1e3a9ec662ff19dd28b79e6ec616d74c | master ]
    3. git log --stat
### Descripción:
    1. Vuelve a una version anterior y posiciona head en esta, las opciones soft y hard especifican de que forma lo hacen, soft deja los cambios actuales en el archivo y hard los borra(precaucion).
    2. Se mueve entre los commits y la version actual(master).
    3. Muestra los cambios entre commits especificando las inserciones y eliminaciones realizadas. 
