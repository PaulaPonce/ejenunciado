### Comandos Git

**1 Creando el repositorio local, desde el pc**
  * crear carpeta donde irán los archivos del proyecto
  * git init #crear un repositorio
  * git remote add origin https://github.com/PaulaPonce/ejenunciado/ #conecta  elrepositorio local con el remoto
  * #se realizan los cambios
  * git status
  * git add . #agrega los cambios al staging área
  * git commit –m “mensaje” #pasa los cambios al repositorio local, crea la versión con un mensaje
(hasta acá estamos en el computador)
  * git push origin master #empuja al repositorio remoto (github)

**2 Creando el repositorio remoto, desde github**
  * Primero creamos un repositorio en github, automáticamente crea un commit
  * git clone https://github.com/PaulaPonce/ejenunciado/ #clona el repositorio remoto a local
  * En sublime abro la carpeta clonada
  * #se realizan los cambios
  * git status
  * git add . #agrega los cambios al staging área
  * git commit –m “mensaje” #pasa los cambios al repositorio local
  * git push origin master #empuja al repositorio remoto (github)

**3 Ramas**
  * git checkout -b new-branch #crea una rama y se posiciona en ella
  * git checkout master #volver a la rama master
  * git branch -d new-branch #elimina la rama
  * git push origin <branch> #sube la rama al repositorio remoto

**4 Actualizar**
  * git pull origin master #actualiza los cambios desde github al repositorio local, baja y fusiona los cambios remotos
  * git merge <branch> #fusionar otra rama a la rama master
  * resolver conflictos
  * git diff <source_branch> <target_branch> #revisar cambios

**5 Reemplazar cambios locales**
  * git checkout -- <filename> #reemplaza los cambios con el último contenido
  * #deshacer todos los cambios locales y commits:
    * git fetch origin 
    * git reset --hard origin/master

**6 gh-pages**
  * git checkout -b gh-pages #crear rama gh-pages
  * git rebase master #actualiza la rama gh-pages con la rama master
  * git push origin gh-pages #subir rama a repositorio remoto
  * git checkout master #regresar a rama master
