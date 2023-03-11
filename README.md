Alta y uso de un nuevo repo en Github.
0.- Una de las tareas previas será dar de alta en github una clave SSH para poder subir y bajar info de github al 
espacio local.
1.- Configurar el usuario y mail en el terminal de VSC: 

git config --global user.name <name>      # Para configurar el nombre de usuario global de trabajo en GIT
git config --global user.email <email>    # Para configurar el email glPobal de trabajo en GIT 
git config user.name                      # Para configurar el nombre de usuario del repo de trabajo en GIT
git config user.email                     # Para configurar el nombre de email del repo de trabajo en GIT
git config --global color.ui auto         # Coloración automática para mayor entendimiento.
git config --list                         # Para listar las opciones de config
git config --global diff.tool vimdiff
git config --global difftool.prompt false


2.- Alta de nuevo repo en Github.com. 

3.- Conexión del WS de trabajo local con el repo GIT

git init                                  # Para inicializar el repo git local
git add README.md                         # Para añadir un archivo README.md que abremos creado en el WS a la Stagging Area
git commit -m "first commit"              # Primer commit de nuestro código en el WS local.
git branch -M main                        # Nos cambiamos a la rama main.
git remote add origin git@github.com:Fran-Delgado/Repo_prueba_GIT.git    # Conexión con el repo remoto.
git push -u origin main                   # Para consolidar el último commit en el repo remoto de github

4.- Comandos para cuando se trabaja en el repo local. 

git status                                # Para saber el estado de nuestros ficheros respecto de la stagging area y 
                                          # la rama en la que estamos. 

git log                                   # Para saber el historial de commits. 
Opciones interesantes de git log:
 
--oneline: 			# muestra cada confirmación en una sola línea, lo que facilita la lectura del historial.
--graph: 			# muestra un gráfico ASCII que representa la relación entre las diferentes ramas y confirmaciones.
--author=<author-name> 		# muestra solo las confirmaciones realizadas por un autor específico.
--since=<date>: 		# muestra solo las confirmaciones realizadas desde una fecha específica.
--until=<date>: 		# muestra solo las confirmaciones realizadas hasta una fecha específica.
--grep=<pattern>: 		# muestra solo las confirmaciones que contienen un patrón específico en el mensaje del commit.
--reverse: 			# muestra el historial de confirmaciones en orden inverso (el commit más antiguo primero).

