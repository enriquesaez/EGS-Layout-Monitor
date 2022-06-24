
# Trabajo con repositorios GIT usando Visual Studio Code y Github
### En Github, elegimos la opción "Nuevo" y creamos el nuevo repositorio: http://github.com/new

![Crear un repositorio](https://github.com/enriquesaez/EGS-Layout-Monitor/blob/master/useful/img-create-repo.png)
&nbsp;

## Usando Visual Studio Code para crear un entorno GIT desde cero
### Accedemos a Terminal de Visual Studio Code y ejecutamos lo siguiente:

- `git init` (solo se ejecuta una primera vez) Esto crea y configura un espacio de trabajo GIT

- `git remote add origin http://[URL del repositorio].git` Con este comando clonamos, hacemos una copia en nuestro local de un proyecto remoto.

- `git push -u origin master` Este comando carga nuestro primer contenido desde el repositorio local al repositorio remoto.

## Crear un nuevo repositorio en Visual Studio Code:**

- Opción Clonar Repositorio

![Clonar un repositorio](https://github.com/enriquesaez/EGS-Layout-Monitor/blob/master/useful/img-clone-repository.png)

- Introducimos la url del repositorio proporcionada por Github
## Trabajo con repositorios
- `git status` 
Muestra el estado del directorio de trabajo local y el área del entorno de ensayo. 
Permite ver los cambios realizados y los archivos en los que Git no va a realizar el seguimiento. 

- `git add nombre_archivo`
Añade al entorno virtual un archivo de nuestro repositorio local, ya sea uno nuevo o un archivo modificado. 
El comando "git add" realiza una puesta en escena ("stage") de los cambios. 

- `git add .`
Añade al entorno virtual todos los ficheros nuevos o modificados de nuestro proyecto local.

- `git commit -m "comentario del commit"`
Con este comando se realiza una captura, una instantánea de los cambios realizados actualmente en el proyecto. 
Previamente a ello siempre habrá que realizarse la opción "git add".

- `git push`
Sube al repositorio remoto todos los cambios producidos en nuestro repositorio local.
La diferencia básica entre **git commit** y **git push** es que el alcance de git commit es el repositorio local, y el de git push es el repositorio remoto. 
El comando git push siempre viene después de ejecutar el comando git commit.

- `git branch`
Muestra las ramas existentes en nuestro repositorio GIT. Normalmente los miembros de un equipo trabajan con una versión (rama o branch) local del repositorio para después subir el trabajo a una rama remota, que finalmente se fusionará (merge) con el repositorio remoto principal.

- `git brach nombre-nueva-rama`
Crea una rama nueva a partir de una copia actual del repositorio principal o de otra rama.

- `git brach -d nombre-rama-para-borrar`
Borra del repositorio remoto una rama.

### Subir al repositorio remoto una nueva rama creada

- `git push --set-upstream origin NOMBRE_RAMA`
&nbsp;
### Identificarse al hacer un commit y su usuario quede registrado como autor del commit

- `global user.email "you@example.com"`

### Guía completa sobre GIT y control de versiones en Español:

**Web:**
- **[Guía - Libro de Git](https://git-scm.com/book/es/v2)**

**Descarga PDF:**
- [Guía -Libro de Git](https://github.com/progit/progit2-es/releases/download/2.1.23/progit.pdf).

