- Vamos a crear una rama llamada dev para esto ejecutamos:

> - `$ git checkout -b dev`

Al ejecutar `$ git status` nos indicara que estamos en la rama dev que acabamos de crear, para poder ver las ramas que tenemos en nuestro repositorio y en cual rama estamos ubicadios debemos ejecutar `$ git branch` y si quieremos ver las ramas con el ultimo commit ejecutamos `$ git branch -v`

- Ahora dentro de la rama dev vamos a crear un archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> y vamos añadirlo y realizar el commit

> - `$ touch style.css`
> - `$ git add .`
> - `$ git commit -m "add file style.css"`

Para poder movernos de rama master ejecutamos `$ git checkout master`, en esta rama al listar los archivos `$ ls -l` podemos ver que no tenemos el archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> por lo que vamos a movernos nuevamente a la rama dev usando `$ git checkout dev`

- Vamos a modificar el archivo <abbr title="Hyper Text Markup Language"> style.css </abbr> agregando el siguiente codigo: 

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