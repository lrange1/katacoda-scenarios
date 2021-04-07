- Para realizar un Merge vamos a llevar los cambios de la rama dev a la rama master, para esto primero debemos ubicarnos en la rama destino, en este caso es la rama master: 

> - `$ git checkout master`

- Ahora realizamos el merge indicando la rama que queremos fusionar

> - `$ git merge dev`

la salida en terminal nos indica que está actualizando los commits mediante la estrategia de Fast-forward

```sh
Updating 7601ec1..5918d8a
Fast-forward
 style.css | 5 +++++
 1 file changed, 5 insertions(+)
 create mode 100644 style.css
```