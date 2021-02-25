Se debe configurar las variables globales de git como el nombre de usuario y el email para esto se deben ejecutar los siguientes comandos.

> - `$ git config --global user.name "nombre usuario" `

> - `$ git config --global user.email "email"`


Configurar el proxy (En caso de ser necesario)

> - `$ git config --global http.proxy "http://usuario_dominio:clave@dominio:port" `

> - `$ git config --global https.proxy "http://usuario_dominio:clave@dominio:port" `


Para poder validar la configuracion realizada podemos ejecutar el comando `$ cat ~/.gitconfig` que nos indicara las variables que hemos configurado. tambien podemos listar todas las configuraciones con el comando `$ git config --list`