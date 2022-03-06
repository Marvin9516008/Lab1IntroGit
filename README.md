# Lab1IntroGit
Laboratorios #1 - (Introducción a Git)
## _Marvin Diaz, Carnet 9516008_

![Universidad Galileo](https://www.galileo.edu/wp-content/themes/galileo-theme/img/logo-header.png)

## ¿Qué es GIT?
El GIT es un sistema de control de versiones.  Un sistema de control de versiones es una porción de un software que da seguimiento al cambio de los archivos durante el tiempo.  Específicamente GIT es un sistema de control de versión distribuida, lo que significa que todos los que trabajen en un proyecto Git tienen una copia del proyecto, no solo el estado actuad de los archivos.

## ¿Porque usar Git?
Permite varios beneficios aun cuando se trabaje de manera individual:
* Permite revertir los cambios, regresando a un punto del tiempo para recuperar una versión anterior del trabajo.
* Una historia completa de todos los cambios
* Documentación de porque los cambios fueron hechos
* Confianza de cambiar cualquier cosa
* Diferentes streams de historia

## ¿Qué es GitHub?
GitHub es un sitio web donde se puede subir una copia del repositorio Git.  Permite que diferentes personas colaboren más fácilmente en un proyecto.  Esto es posible por medio de proveer la localización centralizada para compartir el repositorio.

## ¿Porque usar GitHub?
GitHub es mucho más que un lugar para almacenar los repositorios Git. Permite beneficios adicionales:
- Documentar requerimientos
- Colaborar en diferentes áreas
- Revisar trabajo en desarrollo
- Ver el progreso del equipo

## ¿Cómo crear un Repositorio?
Para crear un nuevo proyecto en GitHub, se debe de seleccionar el signo + situado a la derecha del nombre del usuario situado en la esquina superior de la página.  Luego, hacer clic en la opción de lista de “Nuevo Repositorio”.  Posteriormente se despliega una forma de “Nuevo Repositorio”.  
Lo primero que se debe hacer es crear el repositorio con el nombre de usuario o con el nombre de la organización.  Si no se tiene acceso directo a una organización se debe de dejar por default el nombre del usuario.  Independientemente, se tiene la opción de transferir el proyecto.  
El paso siguiente es de dar un nombre al repositorio.  El nombre debe ser letras, números, hypens, y/o guion bajo.  Después de ingresar el nombre se debe decidir si hacer el repositorio Publio o Privado.  Repositorios privados pueden ser vistos únicamente por usuarios que uno invite específicamente como colaboradores.
La decisión final que se debe tomar al crear un repositorio es de si se debe inicializarlo con un archivo solo de lectura seleccionando la casilla.

## Agreagando Colaboradores
Ya creado e inicializado el repositorio, el siguiente paso es de agregar colaboradores.  Si se creó el repositorio como público, no se necesita agregar colaboradores, especialmente si se está trabajando con gente ocasionalmente.

## Lista de principales comandos GIT

## _Configuración de Git & INIT_
* Creando un nuevo repositorio de Git a partir de un directorio existente:

git init [directorio]

* Clonar un repositorio (local o remoto a través de HTTP):

git clone [repo / URL]

* Clonar un repositorio en una carpeta especifica en su equipo local:

git clone [repo / URL] [carpeta]

## _Configuración de Git_

* Adjuntar un nombre de autor a todas las confirmaciones que aparecerán en el historial de versiones:

git config --global user.name "[nombre apellido]"

* Adjuntar una dirección de correo electrónico a todas las confirmaciones del usuario actual:

git config --global user.email "[email_address]"

* Aplicar la coloración automática de la línea de comandos de Git  que facilita realizar un seguimiento y revisar los cambios del repositorio:

git config --global color.ui auto

* Para crear un acceso directo (alias) para un comando git:

git config --alias global. [alias_name] [git_command]

* Establecer un editor de texto predeterminado:

git config --system core.editor [text_editor]

* Abrir el archivo de configuración global de Git:

git config --global --edit

## _Administración de archivos_
* Mostrar el estado del directorio actual (lista de archivos organizados, sin especificar y sin seguimiento):

git status

* Enumerar el historial de confirmación de la rama actual:

git log

* Enumerar todas las confirmaciones de todas las ramas:

git log --all

* Comparar dos ramas mostrando qué confirmaciones de la primera rama faltan en la segunda:

git log [rama1].. [rama2]

* Examinar la diferencia entre el directorio de trabajo y el índice:

git diff

* Explorar la diferencia entre la última confirmación y el índice:

get diff --cached

* Ver la diferencia entre la última confirmación y el directorio de trabajo:

get diff HEAD

## _Git branches_
* Enumerar todas las ramas del repositorio:

git branch

* Enumerar todas las sucursales remotas:

git branch -aa

* Crear una nueva rama con un nombre especificado:

git branch [rama]

* Cambiar a una rama con un nombre especificado (si no existe, se creará una nueva):

git checkout [rama]

* Combinar la rama especificada con la rama actual:

git merge [rama]

## _Stage_
* Cambios de stage para el siguiente commit (stage):

git add [archivo/directorio]

* Organizar todo en el directorio para un commit inicial:

git add

* Realizar snapshots preconfigurados en el historial de versiones con un mensaje descriptivo incluyendo en el comando:

git commit -m "[mensaje_descriptivo]"

## _Deshacer cambios_
* Deshacer los cambios en un archivo o directorio y crear una nueva confirmación con el comando git revert:

git revert [archivo/directorio]


* Restablecer un archivo sin sobrescribir los cambios:

git reset [archivo]

* Deshacer los cambios introducidos después de la confirmación especificada:

git reset [commit]

* Mostrar archivos sin seguimiento que se eliminarán cuando ejecute git clean (haga una ejecución en seco):

git clean -n

* Eliminar archivos sin seguimiento:

Git clean -f

## _Sobrescribiendo historia_
* Reemplazar la última confirmación con una combinación de los cambios preconfigurados y la última confirmación combinada:

git commit --enmendar

* Volver a basar la rama actual con la base especificada (puede ser un nombre de rama, una etiqueta, una referencia a un HEAD o un ID de confirmación):

git rebase [base]

## _Repositorios remotos_
* Crear una nueva conexión a un repositorio remoto (asignando un nombre para que sirva como acceso directo a la dirección URL):

git remote add [nombre] [URL]

* Obtener una branch de un repositorio remoto:

git fetch [remote_repo] [rama]

* Buscar un repositorio y combínelo con la copia local:

git pull [remote_repo]

* Insertar una rama en un repositorio remoto con todas sus confirmaciones y objetos:

git push [remote_repo] [branch]

* Clonar un repositorio (local o remoto a través de HTTP):

git clone [repo / URL]

* Clonar un repositorio en una carpeta especifica en su equipo local:

git clone [repo / URL] [carpeta]





## Bibliografia
Bell, P. a. (2015). Introducing GitHub. Sebastopol, CA: Oreilly.
