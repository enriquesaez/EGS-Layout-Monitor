
# Iniciar nuevo repositorio con Github y Visual Studio Code
	
**En Github >>**
*Crear repo*

**En VS Code**

- `git init` (solo una primera vez)
- `git remote add origin http://[URL del repositorio].git`
- `git push -u origin master`

**O bien, crear repo directamente en VS Code:**
- Clone repository > introducir url del repositorio en Github


**Trabajo basico con repositorios:**

- `git status` <- *Vemos el estado de nuestro repositorio respecto al repo en origen (origin, master...)*
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
