Creando el repositorio desde el pc
•	git init #crear un repositorio
•	git remote add origin
•	#hago los cambios
•	git status
•	git add . #agrega los cambios al staging área
•	git commit –m “mensaje” #pasa los cambios al repositorio local , crea la versión con un mensaje
•	(hasta acá estamos en el computador)
•	git push origin master #empuja al repositorio remoto (github)

Creando el repositorio remoto, desde github
•	Primero creamos un repositorio en github, click en inicializar con un Readme, automáticamente crea un commit
•	git clone link , voy a github y copio el link del repositorio creado
•	En sublime  abro la carpeta clonada
•	#hago cambio
•	Git status
•	Git add .
•	Git commit –m “mensaje”
•	Git push origin master
•	Git pull origin master para bajar los cambios de github
