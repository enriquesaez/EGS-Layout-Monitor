
# Iniciar nuevo repositorio con Github y Visual Studio Code
	
**En http://github.com/nombre_usuario >>**
*Crear repo*

**Usando Visual Studio Code - Crear entorno GIT desde cero**

- `git init` (solo una primera vez) Esto crea y configura un espacio de trabajo GIT

- `git remote add origin http://[URL del repositorio].git` Con este comando clonamos un proyecto / directorio GIT remoto en nuestro entorno local.

- `git push -u origin master` Este comando carga nuestro primer contenido desde el repositorio local al repositorio remoto.

**Crear un nuevo repositorio en Visual Studio Code:**

- Opción Clonar Repositorio

![Image text](https://github.com/enriquesaez/EGS-Layout-Monitor/blob/master/useful/img-clone-repository.png)

-Introducimos la url del repositorio en Github


**Trabajo con repositorios**

- `git status -s`
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