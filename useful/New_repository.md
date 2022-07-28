
# Iniciar nuevo repositorio con Github y Visual Studio Code
	
**En Github >>**
*Crear repo*

**En VS Code**

- `git init` (solo una primera vez)
- `git remote add origin http://[URL del repositorio].git`
- `git push -u origin master`

**O bien, crear repo directamente en VS Code:**
- Clone repository > introducir url del repositorio en Github


**Trabajo con repositorios:**

- `git fetch` <- *Compara el proyecto local con el remoto*
- `git status` <- *Vemos el estado del proyecto local, respecto al proyecto original (origin, master...)*

**Consolida los cambios realizados en el proyecto local a escena (no sube al repositorio remoto):**

- `git add nombre_archivo` <- *Añade un fichero concreto (nuevo o ya existente editado) a "Stage"*
- `git add .` <- *Añade todos los ficheros nuevos o ya existentes editados) a "Stage"*
- `git commit -m "comentario del commit"` <- *Añade el trabajo a escena (Stage) con un comentario*

**Subiendo los cambios al repositorio remoto:**
- `git push` <- *Sube todo el trabajo al repositorio remoto (origin, master)*
- `git status` <- *Volvemos a comprobar que los cambios se han subido correctamente al remoto*

**Trabajo con ramas (branches):**

- `git branch` <- *Muestra nuestras ramas ya existentes en el repositorio remoto*
- `git brach nombre-nueva-rama`  <- *Crea una rama (una copia) de todo el repo remoto en nuestro local*
- `git brach -d nombre-rama-para-borrar` <- *Elimina una rama del repo remoto en nuestro local*

**Subiendo al repo remoto una nueva rama desde el repo local:**

- `git push --set-upstream origin NOMBRE_RAMA`

Las ramas creadas en local y "comiteadas" con git push al repo remoto necesitan ser fusionadas "merge" al repositorio remoto mediante una *Pull Request* y una confirmación posterior. Dependiendo de la configuración del proyecto y los privilegios que disponga determinado usuario del proyecto, esta confirmación de la pull request podrá hacerse efectiva, o bien necesitará de aprobación de un usuario administrador del repositorio.

**Identificarse al hacer commit:**

- `global user.email "you@example.com"`
