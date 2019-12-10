# Git_GitHub_Tutorial
## Comando básicos

Configurar Nombre que salen en los commits
```ssh
	git config --global user.name "Ricardo Marcelo"
```
Configurar Email
```ssh	
	git config --global user.email ricardomarcelo@hotmail.com
```
Carpeta local de nuestro proyecto donde inicializamos un repositorio GIT
```ssh
	git init
```
Clonar un repositorio remoto para trabajarlo localmente desde GitHub
```ssh
	git clone <url>
```
Agregar todos loas archivos modificados al INDEX (Stage)
```ssh
	git add .
```
Aceptamos los cambios del INDEX (Stage) y lo registramos con un comentario en el HEAD
```ssh
	git commit -m "Texto que identifique por que se hizo el cambio (commit)"
```
Retirar un cambio del HEAD
```ssh
	git reset HEAD <archivo>
```
Devuelve el ultimo commit y todos los cambios
```ssh
	git reset --hard HEAD^
```
Devuelve los 2 ultimo commit y todos los cambios
```ssh
	git reset --hard HEAD^^
```
Rollback merge/commit usando su idetificador sha
```ssh
	git log
	git reset --hard <commit_sha>
```
Enviar los cambios del HEAD al repositorio remoto
```ssh
	git push origin master
```
Mostrar los logs de los commits realizados
```ssh
	git log --oneline --graph
```
Muestra lista repositorios
```ssh
	git remote -v
```
Crear una rama (branch)
```ssh
	git branch <nameBranch>
```
Lista los branches
```ssh
	git branch
```
Comando -d elimina el branch y lo une al master
```ssh
	git branch -d <nameBranch>
```
Muestra una lista de todos los tags
```ssh
	git tag
```
Crea un nuevo tags
```ssh
	git tag -a <verison> - m "esta es la versión x"
```
Lista un estado actual del repositorio con lista de archivos modificados o agregados
```ssh
	git status
```
Busca los cambios nuevos y actualiza el repositorio
```ssh
	git pull origin <nameBranch>
```
Cambiar de branch
```ssh
	git checkout <nameBranch/tagname>
```
Une el branch actual con el especificado
```ssh
	git merge <nameBranch>
```
Verifica cambios en el repositorio online con el local
```ssh
	git fetch
```
