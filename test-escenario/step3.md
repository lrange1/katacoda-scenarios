- Para iniciar un proyecto con Git, vamos a crear una carpeta llamada curso-git que va a contener el proyecto, se debe ejecutar:

    > -  `$ mkdir curso-git `

- Luego vamos a ingresar a la carpeta del proyeto he inicializar el proyecto git
 
    > -  `$ cd curos-git `
    > -  `$ git init `

- Crear un archivo <abbr title="Hyper Text Markup Language"> index.html </abbr>

    > -  `$ touch index.html`

- Ejecuta `$ git status ` esto nos indicara que no se ha realizado ningun commit y que existe un archivo, esto indica que aun no tiene nada guardado y que se deben seguir los cambios.

```sh
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
```