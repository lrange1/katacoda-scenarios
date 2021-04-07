- Ahora se debe realizar el seguimiento de los cambios que hemos hecho al agregar el fichero <abbr title="Hyper Text Markup Language"> index.html </abbr>, para ello ejecutamos: 

> -  `$ git add .`

- Al momento de ejecutar nuevamente `$ git status ` los cambios ya se encuentran añadidos, pero aún no tienen commit

```sh
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html
```

- Para agregar un commit debemos ejecutar `$ git commit -m "mensaje"` por ejemplo:

> - `$ git commit -m "add file index.html"`

lo que se ha hecho con este comando es decirle a git que guarde los cambios realizados en este fichero llamado <abbr title="Hyper Text Markup Language"> index.html </abbr> 

- Ahora, vamos a modificar el archivo <abbr title="Hyper Text Markup Language"> index.html </abbr> agregando el siguiente contenido: 

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Curso basico de git SP-Academy</title>
    </head>
    <body>
        <h1>gestion basica de un proyecto</h1>
    </body>
</html>
```

- Si ejecutamos `$ git status ` nos indica que el archivo <abbr title="Hyper Text Markup Language"> index.html </abbr> ha sido modificado, no se ha añadido y aun no tiene seguimiento. 

- Ahora vamos a añadir este archivo en específico para esto debemos ejecutar `$ git add index.html`, a diferencia de `$ git add .` este solo añade el archivo que le indiquemos y si queremos agregar todo ejecutamos `$ git add .`

Finalmente agregamos un commit:

> - `$ git commit -m "Update Index.html"`

Usando el comando `$ git log` podemos ver los commits que se han realizado y si queremos ver de una manera resumida usamos `$ git log --oneline`