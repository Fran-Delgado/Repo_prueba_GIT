Alta y uso de un nuevo repo en Github.
0.- Una de las tareas previas será dar de alta en github una clave SSH para poder subir y bajar info de github al 
espacio local.
1.- Configurar el usuario y mail en el terminal de VSC: 

git config --global user.name <name>      # Para configurar el nombre de usuario global de trabajo en GIT
git config --global user.email <email>    # Para configurar el email global de trabajo en GIT 
git config user.name                      # Para configurar el nombre de usuario del repo de trabajo en GIT
git config user.email                     # Para configurar el nombre de email del repo de trabajo en GIT
git config --list                         # Para listar las opciones de config

2.- Alta de nuevo repo en Github.com. La prueba es con un fichero readme únicamente. 

git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:Fran-Delgado/Repo_prueba_GIT.git
git push -u origin main