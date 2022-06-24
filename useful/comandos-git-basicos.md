
# Trabajo con repositorios GIT usando Visual Studio Code y Github
	
**En Github, opción "Nuevo" y creamos el nuevo repositorio: http://github.com/new >>**

![Image text](https://github.com/enriquesaez/EGS-Layout-Monitor/blob/master/useful/img-create-repo.png)


**Usando Visual Studio Code - Crear entorno GIT desde cero**

- `git init` (solo una primera vez) Esto crea y configura un espacio de trabajo GIT

- `git remote add origin http://[URL del repositorio].git` Con este comando clonamos un proyecto / directorio GIT remoto en nuestro entorno local.

- `git push -u origin master` Este comando carga nuestro primer contenido desde el repositorio local al repositorio remoto.

**Crear un nuevo repositorio en Visual Studio Code:**

- Opción Clonar Repositorio

![Image text](https://github.com/enriquesaez/EGS-Layout-Monitor/blob/master/useful/img-clone-repository.png)

-Introducimos la url del repositorio de Github

**Trabajo con repositorios**

- `git status -s` El comando git status muestra el estado del directorio de trabajo y del área del entorno de ensayo. Permite ver los cambios que se han preparado, los que no y los archivos en los que Git no va a realizar el seguimiento. El resultado del estado no muestra ninguna información relativa al historial del proyecto.
- `git add nombre_archivo`
- `git add .`
- `git commit -m "comentario del commit"`
- `git push`
- `git branch`
- `git brach nombre-nueva-rama`
- `git brach -d nombre-rama-para-borrar`

**Subir al repo una nueva rama creada en Visual Studio**

- `git push --set-upstream origin NOMBRE_RAMA`

**Identificarse al hacer un commit**

- `global user.email "you@example.com"`
