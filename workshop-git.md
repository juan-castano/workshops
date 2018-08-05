# Workshop git-scm

Ahora será usted el encargado de gestionar el repositorio para su proyecto.
Para esto deberá contar con una cuenta en GitHub, Gitlab, Bitbucket o servicio de almacenamiento de código que prefiera.

Deberá usar la consola con el fin de interiorizar el funcionamiento del SCM.

El proyecto lo definiremos de la siguiente manera:

En su repositorio existirán dos ramas:
* __master__ dónde desplegaremos las liberaciones para publicar en producción. Será la rama __stable__
* __devel__ que contendrá todos los cambios de desarrollo que se mezclaran desde las diferentes ramas. Será la rama __unstable__

Este ejercicio recogerá la temática tratada en la capacitación.
***

Se le ha designado para la gestión del repositorio de software del proyecto al cuál está vinculado.

Lo primero será definir una carpeta que contendrá el código fuente e inicializarla para administrar su repositorio allí.

Crear en su servidor de preferencia un repositorio con el nombre que desee y la URL proporcionada deberá indicarla en su repositorio local y así definir dónde se almacenarán sus cambios. `Hint: git remote`

Configurar su nombre de usuario y email para el repositorio con el fin de evitar commits anónimos. `Hint: git config`

Definirá su línea base de desarrollo con los siguientes (su commit inicial desde la rama __master__):
* markdown.md
* loremipsum.md
* config.txt
* american.md


Luego definirá las dos ramas principales del proyecto (master y devel) y hará su primer commit sobre master de allí derivará su rama de devel. 

De __devel__ desprenderá una __nueva rama__ con el nombre que deseé y allí hará nuevos cambios en __TODOS__ los archivos.

__Usted deberá hacer:__
- Para uno de los archivos, sin agregarlo al stage, deberá deshacer los cambios. `git checkout`
- A dos de los archivos, agregarlos al stage y realizar un commit SIN REALIZAR PUSH. `Hint: git add && git commit`
- A otro agregarlo al stage pero deshacer sus cambios. `Hint: git reset HEAD name_file`
- Agregar un nuevo archivo y no rastrearlo.

Luego de esto no deben haber cambios pendientes. `Hint: git status`


Nuevamente modifique todos los archivos y esta vez deberá realizar un commit para cada fichero.

Luego el stage deberá quedar sin cambios pendientes

Deberá agregar dos archivos más al repositorio y rastrearlos en commits independientes.

Luego renombrar uno de los archivos y hacer commit a los cambios. `Hint: git mv old_name_file new_name_file`
Luego eliminar el archivo restante y realizar commit. `Hint: git rm name_file`

Deberá publicar sus cambios en el servidor y allí realizar un pull request a la rama de devel. 

Luego en su local cambiar a la rama de devel y allí generar una liberación con commits específicos que ud deberá seleccionar a su gusto y estos cambios materializarlos en la rama master local. `Hint: git cherry-pick`

En su rama master definir una etiqueta de liberación (p.ej. v0.1.0, release-20180803, etc) y publicar esos cambios en su rama master remota. `Hint: git tag`

### Repetir el ciclo hasta tener (3) liberaciones etiquetadas en master
