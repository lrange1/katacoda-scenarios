Se deben configurar las variables globales de git como el nombre de usuario y el email. Para esto se deben ejecutar los siguientes comandos.

> - `$ git config --global user.name "nombre usuario" `

> - `$ git config --global user.email "email"`

Un ejemplo de los comandos podria ser:

> - `$ git config --global user.name "sperez" `
> - `$ git config --global user.email "sperez@gmail.com"`


Configurar el proxy (En caso de ser necesario), para este caso no se requiere la configuración del proxy

> - `$ git config --global http.proxy "http://usuario_dominio:clave@dominio:port" `

> - `$ git config --global https.proxy "http://usuario_dominio:clave@dominio:port" `

un ejemplo de los comandos usados podrian ser:

> - `$ git config --global http.proxy "http://sperez:seguridad2020*@picis:80" `

> - `$ git config --global https.proxy "http://sperez:seguridad2020*@picis:80" `


Para poder validar la configuración realizada podemos ejecutar el comando `$ cat ~/.gitconfig` que nos indicara las variables que hemos configurado. Tambien podemos listar todas las configuraciones con el comando `$ git config --list`