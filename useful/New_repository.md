
# Iniciar nuevo repositorio con Github y Visual Studio Code
	
**Directamente en la herramienta web de Github:**
- Utilizar la opción de *Crear repositorio*

**En consola de comandos Git Batch o en Terminal de Visual Studio Code**

- `git init` (solo una primera vez)
- `git remote add origin http://[URL del repositorio].git`
- `git push -u origin master`

**O bien, crear un repositorio a través de la interfaz de Visual Studio Code:**
- Clone repository > *url del repositorio en Github*

# Trabajando con comandos GIT

**Comandos para visualizar el versionado de un proyecto:**

- `git fetch` <- *Compara el proyecto local con el remoto*
- `git status` <- *Vemos el estado del proyecto local, respecto al proyecto original (origin, master...)*


**Consolidando los cambios realizados en el proyecto local a escena (NO sube los cambios al repositorio remoto):

- `git add nombre_archivo` <- *Añade un fichero concreto (nuevo o ya existente editado) a "Stage"*
- `git add .` <- *Añade todos los ficheros nuevos o ya existentes editados) a "Stage"*
- `git commit -m "comentario del commit"` <- *Añade el trabajo a escena (Stage) con un comentario*

**Subiendo los cambios al repositorio remoto:**

- `git push` <- *Sube todo el trabajo al repositorio remoto (origin, master)*
- `git status` <- *Volvemos a comprobar que los cambios se han subido correctamente al remoto*

# Trabajando con ramas (branches)

**Visualización, creación y borrado de ramas:**

- `git branch` <- *Muestra nuestras ramas ya existentes en el repositorio remoto*
- `git brach nombre-nueva-rama`  <- *Crea una rama (una copia) de todo el repo remoto en nuestro local*
- `git brach -d nombre-rama-para-borrar` <- *Elimina una rama del repo remoto en nuestro local*

**Subir al repositorio remoto una nueva rama creada en el repositorio local:**

- `git push --set-upstream origin NOMBRE_RAMA`


# Consideraciones sobre la subida de ramas y Pull Request

Las ramas generadas en nuestro proyecto local y cuyos cambios ya han sido "comiteados", subidos con `git push` a una rama remota del repositorio remoto, pueden añadirse finalmente, fusionarse, al repositorio remoto. Esta fusión (merge) se efectua mediante *Pull Request*, una petición que puede realizarse facilmente en entornos web como GitHub o GitLab, en la que, a través de la interfaz de estas herramientas online, solicitamos incluir una rama con la copia de nuestro trabajo y los cambios producidos, en el repositorio remoto principal. 

Además, se necesitará una confirmación posterior de los mencionados cambios que van a fusionarse el en repositorio. Una vez aprobada y confirmada esta petición *pull request*, los cambios ya deberían estar consolidados y verse reflejados en el repositorio remoto, es decir: el commit o commits de los que se componga el trabajo realizado, los diferentes ficheros afectados, los nuevos ficheros o directorios añadidos, el código fuente añadido o editado, la fecha de inclusión y el usuario autor de estos cambios.

Dependiendo de la configuración del proyecto y los privilegios que disponga determinado usuario, esta confirmación de la pull request podrá hacerse efectiva directamente por el propio usuario (nuevamente a través de GitHub o GitLab) en el caso de que dicho usuario disponga de los permisos pertinentes. En el caso de que las aprobaciones de pull request en un proyecto estén sujetas a una aprobación superior de un usuario administrador del repositorio, será dicho usuario administrador el que revisará y aceptará (o rechazará) la petición de la inclusión del trabajo en el repositorio remoto.

**Identificarse al hacer commit:**

- `global user.email "you@example.com"`
