Primero vamos a instalar gitflow ejecutando: 

> - `$ apt-get install git-flow`

Para inicializar un repositorio con GitFlow vamos a crear una nueva carpeta que va a contener nuestro proyecto:

> - `$ cd`
> - `$ mkdir proyecto-gitflow`
> - `$ cd proyecto-gitflow`

Ahora vamos a ejecutar:

> - `$ git flow init`

debemos indicarle el nombre de la rama master y la rama develop que qeramos en este caso el nombre de la rama master queda igual y la rama develop quedara dev, lo demas lo dejamos por defecto, la salida en terminal sera: 

```sh
Initialized empty Git repository in /home/scrapbook/tutorial/proyecto-gitflow/.git/
No branches exist yet. Base branches must be created now.
Branch name for production releases: [master] master
Branch name for "next release" development: [develop] dev


How to name your supporting branch prefixes?
Feature branches? [feature/] 
Bugfix branches? [bugfix/] 
Release branches? [release/] 
Hotfix branches? [hotfix/] 
Support branches? [support/] 
Version tag prefix? [] 
Hooks and filters directory? [/home/scrapbook/tutorial/proyecto-gitflow/.git/hooks]
```

Para la creación de una rama FEATURE ejecutamos el comando `$ git flow feature start [nombre de la rama]` de igual forma si queremos crear una rama RELEASE vamos a ejecutar `$ git flow release start [nombre de la rama]`

En este caso vamos crear una rama Feature que va a partir de la rama dev para esto debemos ubucarnos en la rama dev y ejecutar el comando:

> - `$ git flow feature start Feature`

De esta manera ya tenemos un proyecto gestionado con GitFloW