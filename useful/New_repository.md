
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


**Consideraciones sobre ramas:**

Las ramas generadas en nuestro proyecto local y cuyos cambios ya han sido "comiteados", subidos con `git push` a una rama remota del repositorio remoto, pueden añadirse finalmente, fusionarse al repositorio remoto. Esta fusión (merge) se efectua mediante una *Pull Request*, una petición en la que solicitamos incluir la copia de nuestro trabajo y los cambios producidos al repositorio remoto principal. 

Además, se necesitará una confirmación posterior de los mencionados cambios que van a fusionarse el en repositorio. Una vez aprobada y confirmada esta petición *pull request*, los cambios ya deberían estar consolidados y verse reflejados en el repositorio remoto: el commit o commits de los que se componga el trabajo realizado, los ficheros afectados, la fecha de inclusión y el usuario del proyecto autor de estos cambios.

Dependiendo de la configuración del proyecto y los privilegios que disponga determinado usuario, esta confirmación de la pull request podrá hacerse efectiva directamente por el propio usuario, o bien necesitará de aprobación y confirmacion de un usuario administrador del repositorio.

**Identificarse al hacer commit:**

- `global user.email "you@example.com"`
