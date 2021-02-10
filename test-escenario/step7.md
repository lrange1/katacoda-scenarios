- Los conflictos en git se crean principalmente al intentar realizar un merge entre ramas cuando se realizan los cambios en la misma linea, por ejemplo si tenemos la rama dev y la rama fix-cambio y modificamos la misma linea de codigo al intentar fusionar con master se va a crear un conflicto, para lo cual debemos resolverlo manualmente.

- Para esto vamos a ubicarnos en la rama master y crear una rama llamada fix-cambio apartir de esa rama:

> - `$ git checkout master`
> - `$ git checkout -b fix-cambio`

- Ahora modicamos el archivo <abbr title="Hyper Text Markup Language"> index.html </abbr> con lo siguiente: 

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Curso basico git SP-Academy Sophos</title>
    </head>
    <body>
        <h1>gestion basica de un proyecto</h1>
    </body>
</html>
```

Tenemos que añadir y realizar el commit sobre este cambio usando:

> - `$ git add . && git commit -m "primer cambio sobre index"`


- Ahora vamos a ubicarnos en la rama dev y modificar el archivo <abbr title="Hyper Text Markup Language"> index.html </abbr> en la misma linea colocando: 

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Curso basico de git Sp-Academy de Sophos solutions</title>
    </head>
    <body>
        <h1>gestion basica de un proyecto</h1>
    </body>
</html>
```

De igual manera tenemos que añadir y realizar el commit sobre este cambio usando:

> - `$ git add . && git commit -m "Update sobre index"`

- Para realizar la fusion no ubicamos en la rama destino en este caso en master y realizamos la fusion de la rama de dev y fix-cambio:

> - `$ git checkout master`
> - `$ git merge dev`
> - `$ git merge fix-cambio`

Al mometo de ejecutar `$ git merge fix-cambio` git nos indica que se ha generado un conflicto, por lo cual debemos solucionaro

```sh
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
```

Si revisamos el archivo <abbr title="Hyper Text Markup Language"> index.html </abbr> git nos muertra en el HEAD el primer cambio seguido de la ultima rama en la cual se realizo el merge

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
<<<<<< HEAD
        <title>curso basico de git para Sp-Academy de Sophos solutions</title>
=======
        <title>Curso basico git SP-Academy Sophos</title>
>>>>>> fix-cambio
    </head>
    <body>
        <h1>gestion basica de un proyecto</h1>
    </body>
</html>
```


Para solucionarlo debemos corregir el cambio indicando cual es la linea de codigo que deberia ir, para este ejemplo el codigo quedaria de la siguiente manera: 

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Curso basico de git para SP-Academy de Sophos Solutions</title>
    </head>
    <body>
        <h1>gestion basica de un proyecto</h1>
    </body>
</html>
```

- Finalmente debemos ejecutar 

> - `$ git add . && git commit -m "merge"`

- Para realizar una revision de la ramas y los cambios que se han realizado podemos usar el comando 

> - `$ git log --oneline --decorate --all --graph`