Git, CONFIGURACIÓN (7-4-2022).
`(git-scm.com/downloads)`
___
* `git config --global core.editor "code --wait"` :  Le indicamos a Git que VSCode es nuestro editor por defecto.

* `git config --global -e` : Ver el archivo de configuración global.

* `git config -h` : Muestra todas las opciones de configuración.

Git, PRINCIPALES COMANDOS.
___
* `git init` : Inicializar el git en el camino donde lo ejecutamos. Donde queremos crear nuestro repositorio.

* `git config --global user.name "Nombre"`
* `git config --global user.email "nombre@gmail.com` : Esta información se usa cuando se creen los commints.

* `git status`: Muestra el estado general del proyecto. Archivos agregados, eliminados, modificados, etc.

* `git add fichero1` : Agrega fichero1 al staging area para luego hacerles el commit (`git add .` agrega todo). 

* `git commit -m "mensage"` : Ejecuta el commit con los ficheros que estén en el staging area.

* `git log` : Ver el historial de cambios (los commits realizados).

* `git log --oneline` : Igual a `git log` pero da un resultado más compacto.

* `git log --online -graph` : Muestra las ramas de una forma más gráfica.

* `git diff` : Muestra la diferencia, en cuanto a contenido, de un archivo.

* `git diff` *`hash1`* *`hash2`* : Muestra la diferencia entre dos commits.

* `git restore --staged fichero` : Quita un fichero del staging area.

* `git checkout` *`hash`* : Regresamos al commit representado por el hash.

* `git checkout master` : Regresamos al commit último y descartamos el regreso a un commit anterior.

* `git restore` : Deshacer cambios de los archivos si aún no se ha hecho commit.

* `git rm archivo` : Borra un archivo y agrega el cambio en el stage.

* `git mv nombre1 nombre2` : Mueve o renombra un archivo y agrega el cambio en el stage.


RAMAS
___

* `git branch` : Muestra las ramas que hay creadas actualmente.

* `git brach nombre_rama` : Crea una rama nueva.

* `git checkout nombre_rama` : Movernos a otra rama.

* `git switch nombre_rama` : Movernos a otra rama.

UNIR DOS RAMAS
___

Si tenemos dos ramas (*Master* y *Rama1*) y queremos unir los cambios de *Rama1* a la rama *Master*, parados en *Master* ejecutamos:
* `git merge rama1` : Une los cambios de *rama1* a la rama *Master*.

GITHUB
___
1. Crear una cuenta en GitHub.
2. Crear repositorio.
3. Agregar en nuestro Git la dirección del nuevo repo en GitHub: `git remote add origin https://github.com/...` (crea un repo remoto).

* `git push -u origin master` : Subir los cambios al repositorio.

* `git remote -v` : Comprobar.

* `git pull origin master` : Baja los cambios del repositorio.



