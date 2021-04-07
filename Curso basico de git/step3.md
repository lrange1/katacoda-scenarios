- Para iniciar un proyecto con Git, vamos a crear una carpeta llamada curso-git que va a contener el proyecto, se debe ejecutar:

    > -  `$ mkdir curso-git `

- Luego vamos a ingresar a la carpeta del proyecto he inicializar el proyecto git
 
    > -  `$ cd curso-git `
    > -  `$ git init `

- Crear un archivo <abbr title="Hyper Text Markup Language"> index.html </abbr>

    > -  `$ touch index.html`

- Al ejecutar `$ git status ` nos indicara que no se ha realizado ningún commit y que existe un archivo, esto indica que aún no tiene nada guardado y que se deben seguir los cambios, la salida en terminal luego de ejecutar el comando es la siguiente:

```sh
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
```