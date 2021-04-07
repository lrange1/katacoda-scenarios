### Flujo de trabajo con Git

Un repositorio local de git está compuesto en tres partes el primero es el directorio de trabajo que es el que contiene todos los archivos () la segunda parte es el Index que es la zona intermedia, donde se añaden los cambios que van a ser subidos al repositorio remoto, y la tercera parte es el Head el cual es un apuntador al último commit que se realiza. 

### Glosario de comandos Git
                    
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



### Que es GitFlow

GitFlow es una estrategia estándar para la gestión de ramas, que facilita el control de cambios en tareas de desarrollo en paralelo y promueve la alta calidad en las entregas de nuevas funcionalidades. GitFlow también es el nombre de una herramienta basada en Git que reduce el número de pasos (comandos que requieren ser ejecutados) en el proceso de control de cambios en la estrategia misma (GitFlow)


### Glosario de comandos en GitFlow
                    
Comando | Descripcion
------------- | -------------
`$ git flow init`  | Inicializar repositorio con GitFlow
`$ git flow feature start [FEATURE_NAME]` | Creación de rama feature
`$ git flow feature publish [FEATURE_NAME]`| Publicación de la rama en el repositorio de código fuente (GitHub, Azure repositorios, etc)
`$ git flow feature pull origin [FEATURE_NAME]` | Halar nuevos cambios desde el repositorio de código fuente (GitHub, Azure repositorios, etc)
`$ git push origin feature/[FEATURE_NAME]` | Subir nuevos cambios al repositorio de código fuente (GitHub, Azure repositorios, etc)
`$ git reset --soft [BASELINE COMMIT ID]` | Integrar todos los feature en uno solo Commit
`$ git flow feature finish [FEATURE_NAME]` | Finalizar la rama feature y promocionar los cambios a la rama dev
`$ git flow push origin develop` | Subir los cambios de la rama dev al repositorio de código fuente (GitHub)