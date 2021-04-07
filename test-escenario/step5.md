Una rama Git es simplemente un apuntador móvil apuntando a una confirmación (Commit). La rama por defecto de Git es la rama master, pero esto ha cambiado un poco y en muchos proyecto git se encuentra como la rama main. Con la primera confirmación de cambios que realicemos(commit), se creará esta rama principal master apuntando a dicha confirmación. En cada confirmación de cambios que realicemos, la rama irá avanzando automáticamente.

- Vamos a crear una rama llamada dev para esto ejecutamos:

> - `$ git checkout -b dev`

NOTA: Al ejecutar `$ git status` nos indicara que estamos en la rama dev que acabamos de crear, para poder ver las ramas que tenemos en nuestro repositorio y en cual rama estamos ubicados debemos ejecutar `$ git branch` y si queremos ver las ramas con el ultimo commit ejecutamos `$ git branch -v`

- Ahora dentro de la rama dev vamos a crear un archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> y vamos a añadirlo y realizar el commit

> - `$ touch style.css`
> - `$ git add .`
> - `$ git commit -m "add file style.css"`

Para poder movernos de rama master ejecutamos `$ git checkout master`, en esta rama al listar los archivos `$ ls -l` podemos ver que no existe el archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> por lo que vamos a movernos nuevamente a la rama dev usando `$ git checkout dev`

- Vamos a modificar el archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> agregando el siguiente código: 

```css
h1 {
font-size: 36px;
color: #000;
font-family: 'Open Sans';
}
```

Nuevamente añadimos y realizamos el commit para el seguimiento: 

> - `$ git add style.css`
> - `$ git commit -m "Update file style.css"`