# campus-git-docker
Práctica Git &amp; Docker

1. Bajar y ejecutar la imagen de Docker llamada "hello-world":
docker run hello-world


2. Bajar y ejecutar imagen de SQL server, con los parámetros necesarios para conexión y persistencia de datos:

docker run -e "ACCEPT_EULA=Y"
-e "SA_PASSWORD=yourStrong(!)Password"
-p 1433:1433
-v C:\Users\a875026\Documents\campus-git-docker\data:\var\opt\mssql\data  
-d mcr.microsoft.com/mssql/server:2019-CU15-ubuntu-20.04


3. Comandos necesarios de git para subir cambios al repo

Validar el estatus:
$ git status

Agregar los cambios al area staged:
$ git add "README.md"

Hacemos commit la cantidad de veces que sea necesario:
$ git commit -m "Nombre del commit."

Hacemos push:
$ git push origin main
