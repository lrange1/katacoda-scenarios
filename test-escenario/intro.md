### Flujo de trabajo con Git

Hola esto lo cambio yo!!
Un repositorio local de git está compuesto en tres partes el primero es el directorio de trabajo que es el que contiene todos los archivos () la segunda parte es el Index que es la zona intermedia, donde se añaden los cambios que van a ser subidos al repositorio remoto, y la tercera parte es el Head el cual es un apuntador al último commit que se realiza. 

### Glosario de comandos
                    
Comando | Descripcion
------------- | -------------
`$ git help`  | Muestra los comandos más usados en git
`$ git init`  | Crea localmente un repositorio
`$ git add + path ` | Agrega al repositorio los archivos indicados
`$ git commit -m "mensaje"` | Hace el commit sobre los archivos
`$ git push origin NombreDeBranch ` | Se usa para subir los archivos al repositorio remoto
`$ git branch ` | Muestra lista de las branches
`$ git checkout -b NombreDeBranch ` | Crea un nuevo branch
`$ git checkout NombreDeBranch ` | Se usa para moverse entre branch 
`$ git clone URL ` | Clona un repositorio
`$ git pull origin NombreDeBranch ` | Hace una actualización bajando los cambios del repositorio remoto al local
`$ git merge NombreDeBranch ` | Se usa para fusionar dos ramas
